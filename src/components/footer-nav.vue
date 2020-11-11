<template>
  <div id="footer">
    <div class="footer">
      <div class="container">
        <div class="siteinfo">
          <ul class="nav-footer">
            <li class='first_li'>
              <h3>订单服务 </h3>
              <ul>
                <!---->
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/instruction">购买指南</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/payment">支付方式</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/delivery">送货政策</a>
                </li>
              </ul>
            </li>

            <li class='first_li'>
              <h3>服务支持 </h3>

              <ul>
                <!---->
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/instruction">售后服务</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/payment">维修门店</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/delivery">零售门店</a>
                </li>
              </ul>
            </li>

            <li class='first_li'>
              <h3>自助服务  </h3>
              <ul>
                <!---->
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/instruction">热点咨询</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/payment">预约购买</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/delivery">订单物流</a>
                </li>
              </ul>
            </li>

            <li class='first_li'>
              <h3>媒体中心  </h3>
              <ul>
                <!---->
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/instruction">新闻动态</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/payment">官方视频</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/delivery">图片资源</a>
                </li>
              </ul>
            </li>

            <li class='first_li'>
              <h3>关于公司  </h3>
              <ul>
                <!---->
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/instruction">公司简介</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/payment">加入我们</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/delivery">联系我们</a>
                </li>
              </ul>
            </li>

            <li class='first_li'>
              <h3>关注我们  </h3>
              <ul>
                <!---->
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/instruction">新浪微博</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/payment">官方微信</a>
                </li>
                <li class='last_li'>
                  <a _ href="//www.smartisan.com/support/#/delivery">官方贴吧</a>
                </li>
              </ul>
            </li>
          </ul>

          <ul class="service">
            <li class="tel">400-626-5666</li>
            <li class="time">周一至周日 9:00-18:00（仅收市话费）</li>
            <li class="online">
              <a href="//www.smartisan.com/support/#/self-service"><span class="smartisan-icon info-question"></span>在线帮助</a>
            </li>
          </ul>
        </div>
        <div class="copyright">
          <h4>Copyright ©, Smartisan Digital Co., Ltd. All Rights Reserved.</h4>
          <h5 class="company">北京锤子数码科技有限公司</h5>
          <ul class="privacy">
            <li>
              <a href="//www.smartisan.com/support/#/agreement">法律声明</a>
            </li>
            <li>
              <a href="//www.smartisan.com/support/#/privacy">隐私条款</a>
            </li>
            <li class="devstore">
              <a href="http://dev.smartisan.com/">开发者中心</a>
            </li>
          </ul>
          <h6>
            <a href="http://www.miibeian.gov.cn/" target="_blank">
              <span>京ICP备14041720号-1</span>
              <span>京ICP证140622号</span>
              <span>京公网安备11010502025474</span>
            </a>
          </h6>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
</script>

<style>
  .footer {
    background: #fafafa;
    border-top: 1px solid #e6e6e6;
    display: block;
  }

  .container {
    width: 1220px;
    margin-left: auto;
    margin-right: auto;
  }

  .footer .siteinfo {
    height: 100px;
    padding: 100px 0 32px;
    border-bottom: 1px solid #e6e6e6;
    position: relative;
  }

  .footer .copyright {
    color: #434d55;
    font-size: 12px;
    padding: 40px 0;
  }

  .nav-footer h3 {
    color: #646464;
    font-size: 12px;
    padding: 0 0 14px;
  }

  .nav-footer a {
    color: #969696;
  }

  .first_li {
    width: 149px;
    line-height: 1;
    float: left;
  }

  .last_li {
    color: #c3c3c3;
    font-size: 12px;
    padding: 6px 0;
  }

  .service {
    float: right;
    position: absolute;
    right: 0;
    overflow: hidden;
    line-height: 34px;
  }

  .footer .service .tel {
    text-align: right;
    font-size: 30px;
    line-height: 1;
    cursor: default;
    color: #646464;
    top: -2px;
    position: relative;
  }

  .service .time {
    clear: both;
    width: 241px;
    font-size: 12px;
    line-height: 18px;
    color: #c3c3c3;
    text-align: right;
  }

  .footer .service li.online a {
    float: right;
    width: 102px;
    height: 32px;
    line-height: 32px;
    background: linear-gradient(#fcfcfc, #f5f5f5);
    cursor: pointer;
    font-size: 14px;
    padding: 0 0 0 26px;
    margin-top: 8px;
    text-align: left;
    color: #5079d9;
    border: 1px solid #dcdcdc;
    border-radius: 5px;
  }

  .footer .copyright h4, .footer .copyright h5 {
    float: left;
    height: 15px;
    line-height: 15px;
    color: #757575;
  }

  .footer .privacy {
    float: left;
    margin: 0 0 0 12px;
  }

  .footer .privacy li {
    float: left;
    line-height: 12px;
    padding: 1px 10px 0;
    border-left: 1px solid #ccc;
  }

  .footer .privacy li a {
    color: #5079d9;
    cursor: pointer;
    transition: all .15s ease-out;
    text-decoration: none;
  }

  .footer .copyright h6 {
    clear: both;
    padding: 10px 0 0;
    height: 15px;
  }

  .footer .copyright h6 a {
    color: #bdbdbd;
    font-size: 12px;
    height: 12px;
    line-height: 1;
  }

  .footer .copyright h6 span {
    margin-right: 20px;
  }

</style>
