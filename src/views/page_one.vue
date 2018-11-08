<template>
<div class='main'>
				<div class="store-content ng-scope">
						<div class="sku-box ">
							<div class="gray-box clearfix ">
								<div class="cover">
									<a href="#/item/100030901">
										<img src="https://resource.smartisan.com/resource/90063f11ceb49210bc3d4375b830f262.jpg?x-oss-process=image/resize,w_417/quality,Q_100/format,webp">
									</a>
								</div>
								<div class="story-content">
									<div class="share">
										<h2 class="hide-row"><a href="#" class="ng-binding">坚果 Pro 钢化玻璃手感膜“足迹系列” 公交车</a></h2>
										<h4 ng-if="item.subtitle" class="ng-binding ng-scope">进口钢化玻璃材质、提供高强度保护</h4>
									</div>
									<div class="story">
										<p class="ng-scope"><span  class="ng-binding">
											1947 年 5 月 28 日那天，37  岁的纽约公交车司机威廉·西米洛连同他的 No. 1310 公交车一同人间蒸发，没有人知道他去了哪里。他的老婆和孩子坐立不安，城中谣言四起，他们甚至认为西米洛十有八九出了意外。</span>
										</p>
										<p class="ng-scope"><span  class="ng-binding">
											然而所有人都猜错了。28 日的清晨，纽约阳光灿烂，西米洛像过去的 17 年一样，开着公交车，从车站驶出，看着眼前的场景，他觉得厌倦至极，他已经走了太多次同样的路，见过太多次同样的人、同样的站牌、同样的硬币。做点不一样的事情吧，有个念头在他脑中闪过。</span>
										</p>
										<p class="ng-scope">
											<span  class="ng-binding">
												在冲动还没有冷却的瞬间，西米洛改变了车的路线，在熟悉的路口，他选择了左转……
											</span>
											<a ng-if="$last" href="#" class="ng-scope">阅读全文></a>
										</p>
									</div>
									<div class="info">
										<div class="price discount ng-scope">
											<span class="normal">限时秒杀</span> 
											<span class="highlight">¥ <i class="ng-binding">49.00</i></span> 
											<span class="origin">¥ <i class="ng-binding">99.00</i></span>
										</div>
										<span class="jianguo-blue-main-btn big-main-btn" >
											<a href="#/item/100030901"  class="ng-scope">现在购买</a>
										</span>
								</div>
							</div>
						</div>
				</div>
				
				
			<service></service>
				
			</div>
	</div>
</template>

<script>
import service from '../components/service'
export default{
	components : {
		service
	}
}
</script>

<style>

			.main{
				    min-height: calc(100vh - 454px);
				    background: #ededed;
				    overflow: hidden;
				    width: 100%;
			}
			.store-content {
				    clear: both;
				    width: 1220px;
				    padding: 0 0 25px;
				    margin: 0 auto;
			}
			.gray-box {
			    	padding: 30px 0 20px;
			        overflow: hidden;
    				margin-bottom: 20px;
    				padding: 30px 0 30px;
    				overflow: hidden;
				    background: #fff;
				    border-radius: 8px;
				    border: 1px solid #dcdcdc;
				    border-color: rgba(0,0,0,.14);
				    -webkit-box-shadow: 0 3px 8px -6px rgba(0,0,0,.1);
				    box-shadow: 0 3px 8px -6px rgba(0,0,0,.1);
			}
			.gray-box .cover{
				float: left;
    			margin: 0 0 0 28px;
			}
			.story-content {
			    float: right;
			    width: 640px;
			    margin: 30px 60px 0 23px;
			}
			.story-content .share{
				    padding-bottom: 18px;
    				overflow: hidden;
			}
		 	.story-content h2 {

			    font-size: 24px;
			    color: #000;
			}
			.story-content h2 a
			{
				color: #000;
			}
			.story-content h4{
				    color: #999;
				    float: left;
				    margin-top: 14px;
			}
			.story-content .story{
				    padding: 26px 0;
    				line-height: 24px;
    				border-top: 1px solid #EEE;
    				border-bottom: 1px solid #EEE;
			}
			.discount span{
				    color: #d44d44;
			}
			.story-content .info{
				    padding: 26px 0 0 0;
				    overflow: hidden;
				    line-height: 40px;
			}
			.story-content .price {
			    float: left;
			    margin-top: 5px;
			}
			.story-content .price .normal{
				    margin-right: 7px;
			}
			.story-content .story a {
			    margin-left: 6px;
			    color: #5079d9;
    			cursor: pointer;
			}
			.story-content .price .highlight {
			    font-weight: 700;
			    margin-left: -3px;
			     color: #d44d44;
			    font-size: 18px;
			}
			.story-content .price i {
			    font-size: 26px;
			}
			.story-content .price.discount .origin {
			    position: relative;
			    margin-left: 8px;
			    font-size: 18px;
			    color: #999;
			}
			.story-content .price.discount .origin i {
			    font-size: 18px;
			}
			.story-content .price.discount .origin:after {
			    position: absolute;
			    content: '';
			    border-top: 2px solid #d44d44;
			    width: 100%;
			    top: 46%;
			    left: 0;
			}
			.info .big-main-btn {
			    float: right;
			    width: 139px;
			}
			.big-main-btn {
			    height: 48px;
			    background: linear-gradient(#799CEA,#567CE6);
    			box-shadow: 0 1px 3px rgba(0,0,0,.1), inset 0 -1px 2px rgba(0,0,0,.2);
    			display: block;
			    padding: 1px;
			    margin: 0 auto;
			    border-radius: 9px;
			    background: #015e94;
			    background: linear-gradient(#5598c9,#2a6da2);
			    text-align: center;
			    text-shadow: rgba(255,255,255,.496094) 0 1px 0;
			    cursor: pointer;

			}
			.info .big-main-btn a {
			    font-size: 16px;
			     height: 44px;
			    line-height: 45px;
			    font-size: 18px;
			    color: #FFF;
			}
</style>