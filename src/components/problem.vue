<template>

				<div class="box box-question">
					<header  class="title-header">
						<h5  class="title">常见问题</h5> 
					</header>
					<div class="panel-content">
						<div class="banner-list clearfix">
							<ul  class="banner-list clearfix">
								<!---->
								<li  class="goumai">
									<h3  class="title">购买指南</h3>
									<!---->
									<ul  class="sub-question clearfix">
										<!---->
										<li >
											<a  href="#">购买渠道</a>
										<li >
											<a  href="#">支付方式</a>
										</li>
										<li >
											<a  href="#">支付时效</a>
										</li>
										<li >
											<a  href="#">分期付款</a>
										</li>
										<li >
											<a  href="#">发票说明</a>
										</li>
										<li >
											<a  href="#">修改发票抬头</a>
										</li>
									</ul>
								</li>
								<li  class="dingdan">
									<h3  class="title">订单物流</h3>
									<!---->
									<ul  class="sub-question clearfix">
										<!---->
										<li >
											<a  href="#">修改订单</a>
										</li>
										<li >
											<a  href="#">发货时效</a>
										</li>
										<li >
											<a  href="#">订单及物流</a>
										</li>
										<li >
											<a  href="#">包邮政策</a>
										</li>
										<li >
											<a  href="#">签收须知</a>
										</li>
									</ul>
								</li>
								<li  class="jishu">
									<h3  class="title">技术支持</h3>
									<!---->
									<ul  class="sub-question clearfix">
										<!---->
										<li >
											<a  href="#">强制重新启动</a>
										</li>
										<li >
											<a  href="#">截屏功能</a>
										</li>
										<li >
											<a  href="#">延长续航时间</a>
										</li>
										<li >
											<a  href="#">定位导航</a>
										</li>
										<li >
											<a  href="#">手机开机激活方法</a>
										</li>
									</ul>
									<ul  class="sub-question clearfix">
										<!---->
										<li >
											<a  href="#">支持耳机接口标准</a>
										</li>
									</ul>
								</li>
								<li  class="shouhou">
									<h3  class="title">售后政策</h3>
									<!---->
									<ul  class="sub-question clearfix">
										<!---->
										<li >
											<a  href="#">手机产品</a>
										</li>
										<li >
											<a  href="#">手机附件</a>
										</li>
										<li >
											<a  href="#">耳机、坚果自拍杆</a>
										</li>
										<li >
											<a  href="#">合作厂商商品</a>
										</li>
										<li >
											<a  href="#">三包权益</a>
										</li>
									</ul>
									<ul  class="sub-question clearfix">
										<!---->
										<li >
											<a  href="#">意外碎屏保修服务</a>
										</li>
										<li >
											<a  href="#">意外损坏保修服务</a>
										</li>
										<li >
											<a  href="#">延长保修服务</a>
										</li>
									</ul>
								</li>
							</ul>
						</div>
					</div>
				</div>

</template>

<script>
</script>

<style>
/*常见问题的样式 start*/
		.content .box {
		    overflow: hidden;
		    z-index: 0;
		    margin-top: 29px;
		    border: 1px solid rgba(0,0,0,.14);
		    border-radius: 8px;
		    background: #fff;
		    box-shadow: 0 3px 8px -6px rgba(0,0,0,.1);
		}
		.box-question .title-header{
			display: block;
		    font-size: 18px;
		    line-height: 60px;
		    color: #9f9f9f;
		    background: #fafafa;
		    border-bottom: 1px solid rgba(0,0,0,.1);
		}
		.box-question .title{			
    		margin-left: 30px;
		}
		.box-question .panel-content{
			    overflow: hidden;
    			transition: all .3s ease-in-out;
		}

		.box-question .banner-list > li {
		    width: 50%;
		    padding: 38px 0 35px 120px;
		    background-repeat: no-repeat;
		    background-size: 54px auto;
		    background-position-x: 35px;
		    background-image: url(http://static.smartisanos.cn/service/assets/images/question-icon.9061b2228768f4b09c58e907f170570b.png);
		    background-image: -webkit-image-set(url(http://static.smartisanos.cn/service/assets/images/question-icon.9061b2228768f4b09c58e907f170570b.png));
		}
		.box .banner-list > li {
		    float: left;
		    box-sizing: border-box;
		    border-right: 1px solid #ececec;
		    border-bottom: 1px solid #ececec;
		}
		.box-question .banner-list > li .title {
		    font-size: 16px;
		    line-height: 1em;
		    margin-bottom: 20px;
		    color: #333;
		}
		.box-question .banner-list > li ul {
		    font-size: 12px;
		    line-height: 1em;
		    color: #999;
		    overflow: hidden;
		    margin-top: 12px;
		}
		.box-question .banner-list > li ul li:first-child {
		    padding-left: 0;
		}
		.box-question .banner-list > li ul li {
		    float: left;
		    padding-left: 16px;
		    position: relative;
		}
		.box-question .banner-list > li ul li:before {
		    content: "\B7";
		    position: absolute;
		    left: 5px;
		}
		.box-question .banner-list > li a {
		    color: #a7a7a7;
		    
		}
		.box-question .banner-list > li a:hover{
			color: #5079d9;
			cursor: pointer;
		    transition: all .15s ease-out;
		    text-decoration: none;
		}
		.box-question .banner-list > li.goumai {
		    background-position-y: 33px;
		}
		.box-question .banner-list > li.dingdan {
		    background-position-y: -232px;
		}
		.box-question .banner-list > li.jishu {
		    background-position-y: -90px;
		}
		.box-question .banner-list > li.shouhou {
		    background-position-y: -344px;
		}
		/*常见问题的样式 end*/
</style>