<template>
	<div class="box box-self">
				<header class="title-header">
					<h5 class="title">自助服务</h5> </header>
					<div class="panel-content">
						<ul class="banner-list clearfix">
							<!---->
							<li class="daodian">
								<img src="../assets/img/img01.png"/>
								<h3 class="title">到店快修</h3>
								<p class="sub-title">线下服务网点信息</p>
								<a href="//www.smartisan.com/support/#/servicelist"></a>
							</li>
							<li class="quanguo">
								<img src="../assets/img/img01.png"/>
								<h3 class="title">发起售后</h3>
								<p class="sub-title">通过 IMEI 号或 SN 号发起售后</p>
								<a href="/service/#/insurance/aftersale"></a>
							</li>
							<li class="query-insurance">
								<img src="../assets/img/img01.png"/>
								<h3 class="title">保修查询</h3>
								<p class="sub-title">激活及保修信息查询</p>
								<a href="/service/#/insurance/query"></a>
							</li>
							<li class="weixiu">
								<img src="../assets/img/img01.png"/>
								<h3 class="title">维修价格</h3>
								<p class="sub-title">手机维修报价查询</p>
								<a href="//www.smartisan.com/support/#/serviceprice"></a>
							</li>
							<li class="fuwu">
								<img src="../assets/img/img01.png"/>
								<h3 class="title">服务政策</h3>
								<p class="sub-title">官方/合作厂商商品售后政策</p>
								<a href="//www.smartisan.com/support/#/service-policy"></a>
							</li>
							<li class="xiaoshou" style="border-right: oldlace">
								<img src="../assets/img/img01.png"/>
								<h3 class="title">销售门店</h3>
								<p class="sub-title">线下体验店信息</p>
								<a href="//www.smartisan.com/support/#/storelist"></a>
							</li>
						</ul>
						<ul class="insurance-list clearfix">
							<li class="broken">
								<img src="http://static.smartisanos.cn/service/assets/images/page-accident.a9f4a086bbbf1cd92544d66cbca9c08b.png"/>
								<div>
								<h3 class="">“屏幕意外摔碎，可以免费更换? ”</h3>
								<p class="">坚果 Pro 意外碎屏保修服务</p>
								<a routerlink="/insurance/info/broken" href="#/insurance/info/broken">进一步了解详情 <span class="smartisan-icon gt"></span></a>
								<a class="cover" routerlink="/insurance/info/broken" href="#/insurance/info/broken"></a>
								</div>
							</li>
							<li class="delay">
								<img src="http://static.smartisanos.cn/service/assets/images/page-delay.575b1578f3bf431242f875914efae311.jpg"/>
								<div>
								<h3 class="">Smartisan 延长保修服务</h3>
								<p class="">Smartisan 手机和坚果 Pro</p>
								<a fragment="delay" routerlink="/insurance/info/broken" href="#/insurance/info/broken#delay">进一步了解详情 <span class="smartisan-icon gt"></span></a>
								<a class="cover" fragment="delay" routerlink="/insurance/info/broken" href="#/insurance/info/broken#delay"></a>
								</div>
							</li>
						</ul>
					</div>
				</div>
</template>

<script>
</script>

<style>
/*常见问题的样式 start*/
		.nav-sub .nav-sub-wrapper:after {
		    content: " ";
		    position: absolute;
		    top: 89px;
		    left: 50%;
		    margin-left: -610px;
		    width: 1220px;
		    background: #e7e7e7;
		    height: 1px;	
		    opacity: 0.1;
		}
		.content .box {
		    overflow: hidden;
		    z-index: 0;
		    margin-top: 29px;
		    border: 1px solid rgba(0,0,0,.14);
		    border-radius: 8px;
		    background: #fff;
		    box-shadow: 0 3px 8px -6px rgba(0,0,0,.1);
		}
		.content .box .title-header {
		    display: block;
		    font-size: 18px;
		    line-height: 60px;
		    color: #9f9f9f;
		    background: #fafafa;
		    border-bottom: 1px solid rgba(0,0,0,.1);
		}
		.content .box .title-header .title {
		    margin-left: 30px;
		}
		.content .box .panel-content {
		    overflow: hidden;
		    transition: all .3s ease-in-out;
		}
		.content .box-self .banner-list li {
		    position: relative;
		    text-align: center;
		    width: 16.666%;
		    height: 270px;
		}
		.box .banner-list > li {
		    float: left;
		    box-sizing: border-box;
		    border-right: 1px solid #ececec;
		    border-bottom: 1px solid #ececec;
		}

		.content .box-self .banner-list li.daodian .title {
		    background-position-x: 70px;
		}
		.content .box-self .banner-list li .sub-title {
		    font-size: 12px;
		    color: #999;
		    line-height: 1em;
		}

		/*清楚浮动*/
		.clearfix:after {
		    visibility: hidden;
		    display: block;
		    font-size: 0;
		    content: " ";
		    clear: both;
		    height: 0;
		}
		.banner-list li:hover{
				box-shadow: 0 0 38px rgba(0,0,0,.08) inset;
    			transition: all .15s ease;
		}
		.banner-list img{
			    margin: 80px auto 30px;

		}
		
		ul li {
		    list-style: none;
		}
		.insurance-list .broken img{
			width: 178px;
			height: 178px;
			margin: auto 50px;
		}
		.insurance-list .delay img{
			width: 138px;
			height: 138px;
			margin: 20px 70px;
		}

		.insurance-list li{
				position: relative;
			    float: left;
			    width: 608px;
			    height: 200px;

		}
		
		.insurance-list li:first-child {
		    border-right: 1px solid #ececec;
		}
		.insurance-list div{
				width: 400px;
			   	position: absolute;
			   	left: 210px;
			   	top: 50px;
			   	text-align: center;
		}
		.insurance-list div h3{
			    font-size: 20px;
			    line-height: 1em;
			    color: #d44d44;
			    margin-bottom: 15px;
		}
		.insurance-list div p{
			    font-size: 14px;
			    line-height: 1em;
			    color: #bbb;
			    margin-bottom: 30px;
		}
		.insurance-list div a{
			    font-size: 14px;
    			line-height: 1em;
		        color: #5079d9;
			    cursor: pointer;
			    transition: all .15s ease-out;
			    text-decoration: none;
		}
		/*常见问题的样式 end*/
</style>