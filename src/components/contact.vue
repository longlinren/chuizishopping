<template>

					<div class="box box-official">
						<header  class="title-header"> 
							<h5  class="title">联系客服</h5> 
						</header>
				
					<div  class="panel-content">
						<ul  class="banner-list clearfix">
							<li  class="wechat ">
								<h3  class="title">微信客服</h3>
								<p  class="time">9:00 - 21:00</p>
							</li>
							<li  class="weibo">
								<h3  class="title">微博客服</h3>
								<p  class="time">9:00 - 24:00</p>
								<a  href="#" target="_blank"></a>
							</li>
							<li  class="online">
								<h3  class="title">在线客服</h3>
								<p  class="time">9:00 - 18:00</p>
								<a  href="#" target="_self"></a>
							</li>
							<li  class="jingdong">
								<h3  class="title">京东客服</h3>
								<p  class="time">9:00 - 24:00</p>
								<a  href="#" target="_blank"></a>
							</li>
							<li  class="tianmao">
								<h3  class="title">天猫客服</h3>
								<p  class="time">9:00 - 24:00</p>
								<a  href="#" target="_blank"></a>
							</li>
						</ul>
					</div>
				</div>		

</template>

<script>
</script>

<style>
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
		.title-header .title{
			margin-left: 30px;
		}
		.content .box .panel-content {
		    transition: all .3s ease-in-out;
		}
		.box-official .banner-list > li.wechat {

		    background-image: url(http://static.smartisanos.cn/service/assets/images/contact-weixin.b59a829fd5f92fb0c7f99b6fac4337fc.png);
		}
		.box-official .banner-list > li.weibo {
		    background-image: url(http://static.smartisanos.cn/service/assets/images/contact-weibo.c74aa193d498f842566db34a76d71dab.png);
		}
		.box-official .banner-list > li.online {
		    background-image: url(http://static.smartisanos.cn/service/assets/images/contact-online.4ed58ce4085d52a86e8b3e59f61a4a8c.png);
		}
		.box-official .banner-list > li.time {
		    background-image: url(http://static.smartisanos.cn/service/assets/images/contact-online.4ed58ce4085d52a86e8b3e59f61a4a8c.png);

		}
		.box-official .banner-list > li.jingdong {
		    background-image: url(http://static.smartisanos.cn/service/assets/images/contact-jd.f4d73a60ff35564bfbe005e4c3f90c40.png);
		}
		.box-official .banner-list > li.tianmao {
		    background-image: url(http://static.smartisanos.cn/service/assets/images/contact-tmall.d7b78b81cef8607acc15a3f5a95812d5.png);
		}
		.box-official .banner-list > li {
		    position: relative;
		    width: 20%;
		    text-align: center;
		    padding: 160px 0 70px;
		    border-bottom: 0;
		    cursor: pointer;
		    background-repeat: no-repeat;
		    background-size: 60px auto;
		    background-position: center 75px;
		}
		.box .banner-list > li {
		    float: left;
		    box-sizing: border-box;
		    border-right: 1px solid #ececec;
		    border-bottom: 1px solid #ececec;
		}
		.box-official .banner-list > li .title {
		    font-size: 16px;
		    line-height: 1em;
		    color: #333;
		    margin-bottom: 12px;
		}
		.box-official .banner-list > li .time {
		    font-size: 12px;
		    line-height: 1em;
		    color: #999;
		}

</style>