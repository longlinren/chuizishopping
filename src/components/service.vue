<template>
	<div class='main'>
		<div>
			<ul class="shopping-info gray-box">
				<li class="online-services" >
					<span class="online"><img src="../assets/img/icon01.png"/></span>
					<h5>在线客服</h5>
					<h6>周一至周日 9:00-18:00</h6></li>
				<li class="online-services" >
					<span class="online"><img src="../assets/img/icon02.png"/></span>
					<h5>7 天无理由退货</h5>
					<h6>7 天无理由退货 请放心购买</h6></li>
				<li class="online-services" >
					<span class="online"><img src="../assets/img/icon03.png"/></span>
					<h5>15 天免费换货</h5>
					<h6>15 天内如遇质量问题 免费换货</h6></li>
				<li class="online-services" >
					<span class="online"><img src="../assets/img/icon04.png"/></span>
					<h5 class="ng-binding">满 150 元免运费</h5>
					<h6>全场使用顺丰快递</h6></li>
			</ul>
		</div>
	</div>
</template>

<script>
</script>

<style>
.gray-box {
		    margin-bottom: 0;
		    overflow: hidden;
		    background: #fff;
		    border-radius: 8px;
		    border: 1px solid #dcdcdc;
		    box-shadow: 0 3px 8px -6px rgba(0,0,0,.1);
		}
		.shopping-info {
		    margin: 10px 0 0 0;
		    overflow: hidden;
		    background: #fff;
		    text-align: center;
		}
.shopping-info li .online-services {
    cursor: pointer;
}
.shopping-info li {
    float: left;
    width: 304px;
    height: 153px;
}

	.shopping-info li span {
	    margin: 33px auto 5px;
	    display: block;
	    width: 32px;
	    height: 36px;
	}
.shopping-info li h5 {
    color: #000;
    font-size: 15px;
    line-height: 25px;
}
.shopping-info li h6 {
    color: #A8A8A8;
    font-size: 12px;
    line-height: 24px;
}
</style>