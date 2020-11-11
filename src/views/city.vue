<template>
  <div>
    <el-form :inline="true" :model="formInline" class="demo-form-inline">
      <el-form-item label="搜索">
        <el-input v-model="formInline.search" placeholder="搜索"></el-input>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="onSubmit">查询</el-button>
      </el-form-item>
    </el-form>
    <el-table
      :data="tableData"
      border
      v-loading="loading"
      element-loading-text="拼命加载中"
      element-loading-spinner="el-icon-loading"
      element-loading-background="rgba(0, 0, 0, 0.8)"
      :span-method="arraySpanMethod"
      style="width: 100%">
      <el-table-column
        prop="province"
        label="省"
        width="150">
      </el-table-column>
      <el-table-column
        prop="city"
        label="市"
        width="150">
      </el-table-column>
      <el-table-column
        prop="zone"
        label="区"
        width="150">
      </el-table-column>
      <el-table-column
        prop="remake"
        label="备注">
        <template slot-scope="scope">
          <template v-if="scope.row.edit">
            <el-input class="edit-input" size="small" v-model="scope.row.remake"></el-input>
          </template>
          <span v-else>{{ scope.row.remake }}</span>
        </template>
      </el-table-column>
      <el-table-column
        prop="publicSubsidy"
        sortable
        label="国补"
        width="150">
        <template slot-scope="scope">
          <template v-if="scope.row.edit">
            <el-input class="edit-input" size="small" v-model="scope.row.publicSubsidy"></el-input>
          </template>
          <span v-else>{{ scope.row.publicSubsidy }}</span>
        </template>
      </el-table-column>
      <el-table-column
        prop="provinceSubsidy"
        sortable
        label="省补"
        width="150">
        <template slot-scope="scope">
          <template v-if="scope.row.edit">
            <el-input class="edit-input" size="small" v-model="scope.row.provinceSubsidy"></el-input>
          </template>
          <span v-else>{{ scope.row.provinceSubsidy }}</span>
        </template>
      </el-table-column>
      <el-table-column
        prop="citySubsidy"
        sortable
        label="市补"
        width="150">
        <template slot-scope="scope">
          <template v-if="scope.row.edit">
            <el-input class="edit-input" size="small" v-model="scope.row.citySubsidy"></el-input>
          </template>
          <span v-else>{{ scope.row.citySubsidy }}</span>
        </template>
      </el-table-column>
      <el-table-column align="center" label="Actions" width="200">
        <template slot-scope="scope">
          <el-button v-if="scope.row.edit" type="success" @click="confirmEdit(scope.row)" size="small"
                     icon="el-icon-circle-check-outline">Ok
          </el-button>
          <el-button v-if="scope.row.edit" class='cancel-btn' size="small" icon="el-icon-refresh" type="warning"
                     @click="cancelEdit(scope.row)">cancel
          </el-button>
          <el-button v-else type="primary" @click='scope.row.edit=!scope.row.edit' size="small" icon="el-icon-edit">
            Edit
          </el-button>
        </template>
      </el-table-column>
    </el-table>
  </div>
</template>
<script>
  import axios from 'axios'
  export default {
    name: "city",
    data() {
      return {
        tableData: [], //table的数据
        originalData: [],//table数据备份
        provinceArr: [], //省份要合并数组 [2,0,1,3,0,0] 代表第一二行合并,第三行不变,第四五六行合并,0代表原本的那一行被合并,因此这个列被消除
        provincePos: 0, //省份要合并数组内容的序号
        cityArr: [], //同上 市
        cityPos: [],
        zoneArr: [],//同上 区
        zonePos: [],
        formInline: { //form表单
          search: ''
        },
        loading: false
      }
    },
    created() {
      this.init()
    },
    methods: {
      init() {
        this.loading = true;
        axios.get('./static/table.json')
          .then(res => {
            this.loading = false;
            this.tableData = res.data.map((v, index) => {
              this.$set(v, 'edit', false) //增加一个新的属性

              //可以修改的属性值,进行添加一个对应的原本值
              v.originalRemake = v.remake;
              v.originalPublicS = v.publicSubsidy;
              v.originalProvinceS = v.provinceSubsidy;
              v.originalCityS = v.citySubsidy;
              return v
            })
            this.originalData = this.tableData;
            this.merage() //合并的方法
          })
          .catch(e => {
            console.log(e)
          })
      },
      cancelEdit(row) {
        //取消编辑,把原本值进行覆盖回来
        row.remake = row.originalRemake
        row.publicSubsidy = row.originalPublicS
        row.provinceSubsidy = row.originalProvinceS
        row.citySubsidy = row.originalCityS
        row.edit = false
        this.$message({
          message: 'The title has been restored to the original value',
          type: 'warning'
        })
      },
      confirmEdit(row) {
        row.edit = false

        //把新的值,覆盖原本值,以防再次修改
        row.originalRemake = row.remake
        row.originalPublicS = row.publicSubsidy
        row.originalProvinceS = row.provinceSubsidy
        row.originalCityS = row.citySubsidy
        this.$message({
          message: 'The title has been edited',
          type: 'success'
        })
      },
      arraySpanMethod({row, column, rowIndex, columnIndex}) {
        if (columnIndex === 0) {
          //第一列的合并方法,省
          const _row_1 = this.provinceArr[rowIndex];
          const _col_1 = _row_1 > 0 ? 1 : 0; //如果被合并了_row=0则它这个列需要取消
          return {
            rowspan: _row_1,
            colspan: _col_1
          }
        } else if (columnIndex === 1) {
          //第二列的合并方法,市
          const _row_2 = this.cityArr[rowIndex];
          const _col_2 = _row_2 > 0 ? 1 : 0;
          return {
            rowspan: _row_2,
            colspan: _col_2
          }
        } else if (columnIndex === 2) {
          //第三列的合并方法,区
          const _row_3 = this.zoneArr[rowIndex];
          const _col_3 = _row_3 > 0 ? 1 : 0;
          return {
            rowspan: _row_3,
            colspan: _col_3
          }
        }
      },
      merage() {
        //要合并的数组的方法
        this.merageInit();
        for (var i = 0; i < this.tableData.length; i++) {
          if (i === 0) {
            //第一行必须存在
            this.provinceArr.push(1);
            this.provincePos = 0;

            this.cityArr.push(1);
            this.cityPos = 0;
            this.zoneArr.push(1);
            this.zonePos = 0;
          }
          else {
            // 判断当前元素与上一个元素是否相同 this.provincePos是provinceArr内容的序号

            //省
            if (this.tableData[i].province === this.tableData[i - 1].province) {
              this.provinceArr[this.provincePos] += 1;
              this.provinceArr.push(0);
            } else {
              this.provinceArr.push(1);
              this.provincePos = i;
            }

            //市
            if (this.tableData[i].city === this.tableData[i - 1].city && this.tableData[i].province === this.tableData[i - 1].province) {
              this.cityArr[this.cityPos] += 1;
              this.cityArr.push(0);
            } else {
              this.cityArr.push(1);
              this.cityPos = i;
            }

            //区
            if (this.tableData[i].zone === this.tableData[i - 1].zone && this.tableData[i].city === this.tableData[i - 1].city && this.tableData[i].province === this.tableData[i - 1].province) {
              this.zoneArr[this.zonePos] += 1;
              this.zoneArr.push(0);
            } else {
              this.zoneArr.push(1);
              this.zonePos = i;
            }
          }
        }
      },
      merageInit() {
        //初始化省市区的合并行的数组
        this.provinceArr = [];
        this.provincePos = 0;
        this.cityArr = [];
        this.cityPos = 0;
        this.zoneArr = [];
        this.zonePos = 0;
      },
      onSubmit() {
        const filterData = this.originalData; //每次过滤之前都要把筛选之前的tableData重置
        this.tableData = filterData.filter(value => {
          if (this.formInline.search === value.province || this.formInline.search === value.city || this.formInline.search === value.zone) {
            return value;
          } else if (this.formInline.search === '') {
            return value;
          } else if (value.province.includes(this.formInline.search) || value.city.includes(this.formInline.search) || value.zone.includes(this.formInline.search)) {
            return value;
          }
        })
        this.merage();
      }
    }
  }
</script>
<style scoped>

</style>
