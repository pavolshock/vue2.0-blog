<template>
	<div id="contain">
		<el-container>
		   <el-header height="76px">
		    <el-row type="flex" align="middle" class="w-1272">
		    	<el-col :span="4">
		    		<a href="#"><img src="../assets/logo.png" width="177" height="42"></a>
		    	</el-col>
		    	<el-col :span="14">
  				  <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
  				  	  <el-submenu index="1">
  					    <template slot="title">首页</template>
  					    <el-menu-item index="1">首页1-大数据分析</el-menu-item>
  					    <el-menu-item index="1">首页2-AI机器学习</el-menu-item>
  					  </el-submenu>
  					  <el-submenu index="2">
  					    <template slot="title">文章</template>
  					    <el-menu-item index="2-1">Js</el-menu-item>
  					    <el-menu-item index="2-2">HTML</el-menu-item>
  					    <el-menu-item index="2-3">Css</el-menu-item>
  					  </el-submenu>
  					  <el-menu-item index="3">专题</el-menu-item>
  					  <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">下载</a></el-menu-item>
  					  <el-submenu index="5">
  					    <template slot="title">视频</template>
  					    <el-menu-item index="5">宫崎骏--千与千寻</el-menu-item>
  					    <el-menu-item index="5">哈尔的移动城堡</el-menu-item>
  					    <el-menu-item index="5">蒸汽男孩</el-menu-item>
  					  </el-submenu>
  					  <el-menu-item index="6">问答</el-menu-item>
  					  <el-submenu index="7">
  					    <template slot="title">关于</template>
  					    <el-menu-item index="7">作者介绍</el-menu-item>
  					    <el-menu-item index="7">Blog简介</el-menu-item>
  					    <el-menu-item index="7">友情链接</el-menu-item>
  					  </el-submenu>
  					  <el-submenu index="8">
  					    <template slot="title">付费内容</template>
  					    <el-menu-item index="8">文章</el-menu-item>
  					    <el-menu-item index="8">视频</el-menu-item>
  					    <el-menu-item index="8">下载链接</el-menu-item>
  					  </el-submenu>
  				  </el-menu>
		    	</el-col>
		    	<el-col :span="6" id="searchIcon" style="height: inherit">
		    	  <ul class="wechatsearch clearfix">
		    	  	<li>
		    			<el-button type="primary" size="small">写文章</el-button>
		    		</li>
		    		<li>
		    			<a href="#">注册</a>
		    		</li>
		    		<li>
		    			<a href="#">登录</a>
		    		</li>
		    		<li>
		    			<a href="">
		    			  <svg width="24" height="24" t="1509603359747" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2786" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M778.748 575.633c-15.732 0-31.641-15.732-31.641-31.817 0-15.82 15.908-31.817 31.641-31.817 23.994 0 39.903 15.997 39.903 31.817 0 15.997-15.908 31.817-39.903 31.817M603.494 575.633c-15.82 0-31.817-15.732-31.817-31.817 0-15.82 15.997-31.817 31.817-31.817 24.17 0 39.903 15.997 39.903 31.817 0 15.997-15.732 31.817-39.903 31.817M962 615.447c0-127.354-127.442-231.153-270.615-231.153-151.612 0-270.879 103.887-270.879 231.153 0 127.705 119.356 231.153 270.879 231.153 31.729 0 63.721-7.911 95.537-15.908l87.364 47.901-23.906-79.628c63.896-48.076 111.621-111.622 111.621-183.516M277.068 360.477c-23.906 0-47.989-15.997-47.989-39.815 0-23.994 24.082-39.727 47.989-39.727 23.906 0 39.727 15.732 39.727 39.727 0 23.818-15.82 39.815-39.727 39.815M499.959 280.847c24.082 0 39.903 15.82 39.903 39.727 0 23.818-15.82 39.815-39.903 39.815-23.818 0-47.724-15.997-47.724-39.815 0-23.994 23.906-39.727 47.724-39.727M671.17 367.156c10.372 0 20.567 0.791 30.762 1.933-27.598-128.32-164.795-223.682-321.416-223.682-175.078 0-318.516 119.268-318.516 270.879 0 87.451 47.724 159.346 127.442 215.068l-31.817 95.8 111.357-55.81c39.815 7.822 71.807 15.908 111.533 15.908 10.020 0 19.951-0.44 29.707-1.143-6.153-21.357-9.844-43.594-9.844-66.797 0.088-139.219 119.531-252.158 270.791-252.158z" p-id="2787"></path></svg>
		    			</a>
		    		</li>
		    		<li>
		    			<a href="#">
		    			  <svg width="20" height="20" t="1510287126901" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2420" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M430.72 782.4C229.44 782.4 66.272 622.08 66.272 424 66.272 225.92 229.44 65.28 430.72 65.28 632 65.28 795.2 225.92 795.2 424 795.2 622.08 632 782.4 430.72 782.4L430.72 782.4ZM1014.016 968 749.728 707.84C818.912 632.64 861.44 533.44 861.44 424 861.44 189.76 668.608 0 430.72 0 192.832 0 0 189.76 0 424 0 657.92 192.832 847.68 430.72 847.68 533.504 847.68 627.776 812.16 701.824 752.96L967.168 1014.08C980.128 1026.88 1001.088 1026.88 1014.016 1014.08 1026.976 1001.6 1026.976 980.8 1014.016 968L1014.016 968Z" p-id="2421"></path></svg>
		    			</a>
		    		</li>
		    	  </ul>
		    	</el-col>
		    </el-row>
		  <!-- 圣杯布局 -->
		  <div id="w_1272" class="w_1272">
		  	<div id="wrap">
				<div id="center" style="text-align: center; height: 76px; line-height: 76px;">
				<a href="#"><img src="../assets/logo.png" width="141" style="margin: 0 auto;display: inline-block; vertical-align: middle;"></a>
				</div>
			</div>
			<div id="left" style="height: 76px; line-height: 76px">
				<div class="dropdown">
  			       <button class="btn btn-default dropdown-toggle" type="button" id="dropdownMenu1" data-toggle="dropdown" aria-haspopup="true" aria-expanded="true" style="color: #999;border-color: #999;">
  			       <span class="glyphicon glyphicon-align-justify" aria-hidden="true"></span>
  			       </button>
  				    <ul class="dropdown-menu" aria-labelledby="dropdownMenu1">
  				      <li><a href="#">Action</a></li>
  				      <li><a href="#">Another action</a></li>
  				      <li><a href="#">Something else here</a></li>
  				      <li role="separator" class="divider"></li>
  				      <li><a href="#">Separated link</a></li>
  				    </ul>
  				  </div>
			</div>
			<div id="right">
				<a href="#" style="float: right; padding-right: 10px">
	    		<svg version="1.1" width="20" height="76" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px" viewBox="0 0 1000 1000" enable-background="new 0 0 1000 1000" xml:space="preserve"><g><path d="M500,600.7c-154.2,0-279.7-125.5-279.7-279.8c0-154.3,125.5-279.8,279.7-279.8c154.3,0,279.9,125.5,279.9,279.8C779.8,475.2,654.3,600.7,500,600.7z M500,64.2c-141.5,0-256.7,115.2-256.7,256.7c0,141.6,115.2,256.7,256.7,256.7c141.6,0,256.8-115.2,256.8-256.7C756.8,179.3,641.6,64.2,500,64.2z"/><path d="M978.5,958.9c-5.3,0-10.1-3.7-11.2-9.1C924.5,754.5,728,612.7,499.9,612.7c-227.3,0-423.7,141.2-467.1,335.7c-1.4,6.2-7.5,10.2-13.8,8.7c-6.2-1.4-10.1-7.5-8.7-13.7c45.7-205,251.6-353.8,489.6-353.8c238.8,0,444.9,149.4,489.9,355.2c1.4,6.2-2.6,12.4-8.8,13.7C980.1,958.8,979.3,958.9,978.5,958.9z"/></g>
				</svg></a>
			</div>
		  </div>
		  </el-header>
		  <!-- 自适应图片不能自适应 -->
		  <div id="carousels" class="carousels">
		  	<el-carousel :interval="5000" arrow="always" height="400px">
    		  <el-carousel-item v-for="(item,index) in slidefont" :key="index">
    		  	<!-- 使用require可以绑定src,否则路径不对 -->
    		  	<div style=" width: 85%; position: absolute; bottom: 20px; left: 5%; color: #fff; overflow: hidden">
    		  	  <p style="font-size: 2.5rem">{{ item.text }}</p>
    		  	  <p style="line-height: 2.5rem">{{ item.val }}</p>
    		  	</div>
    		  	<img :src="require('../assets/0'+ (index+1) +'.jpg')" />
    		  </el-carousel-item>
  			</el-carousel>
		  </div>
		  <!-- 第一栏--精选导读 -->
		  <div style="width: 77%; margin: 15px auto; background-color: #fff">
		  	<div class="clearfix" style="padding: 10px">
		  		<span style="float: left; color: #333; font-size: 18px"">精选导读</span>
		  		<span style="float: right;color: #999; font-size: 12px; font-weight: 300;">更多 ></span>
		  	</div>
		  	<div v-for="(item,index) in 4" style="float: left; width: 25%; padding: 10px">
		  		<a href="#">
		  			<img :src="require('../assets/news' + (index+1) + '.jpg')" width="100%">
		  		</a>
		  	</div>
		  </div>
		  <el-container style="width: 77%; margin: 0 auto">
		    <el-main style="padding: 0; margin-right: 20px">
			  <div class="clearfix" style="padding: 10px; background-color: #fff;margin-bottom: 5px;">
		  	    <span style="float: left; color: #333; font-size: 18px;">精选导读</span>
		  		<span style="float: right;color: #999; font-size: 12px; font-weight: 300;">更多 ></span>
		  	 </div>
		  	<el-row v-for="(item,index) in artitle" style="width: 100%; padding: 20px; background-color: #fff; margin-bottom: 5px;">
			  <el-col :span="8">
			  	<a href="#">
		  			<img :src="require('../assets/news' + (index+1) + '.jpg')" width="100%">
		  		</a>
			  </el-col>
			  <el-col :span="16" style="padding: 15px 15px;">
			  	<div style="padding-bottom: 48px">
			  	  <h4><a href="">{{ item.text }}</a></h4>
			  	  <p>{{ item.val }}</p>
			  	</div>
			  	<div>
			  	  <div class="f_left" style="width: 75%">
			  	  	<a href=""><img style="display: inline-block; border-radius: 12px" src="../assets/01.jpg" width="24" height="24">&nbsp;&nbsp;hackbill&nbsp;&nbsp;&nbsp;</a>
			  	  	<span>
			  	  		<svg style="position: relative; bottom: -0.125em" width="14" height="14" t="1521337956805" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3333" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M915.2 966.4h-768c-38.4 0-64-25.6-64-64v-640c0-38.4 25.6-64 64-64h128V102.4c0-19.2 12.8-32 32-32s32 12.8 32 32v96h384V102.4c0-19.2 12.8-32 32-32s32 12.8 32 32v96h128c38.4 0 64 25.6 64 64v640c0 38.4-32 64-64 64z m0-672c0-19.2-12.8-32-32-32h-96v96c0 19.2-12.8 32-32 32s-32-12.8-32-32V262.4h-384v96c0 19.2-12.8 32-32 32s-32-12.8-32-32V262.4H179.2c-19.2 0-32 12.8-32 32v160h768V294.4z m0 224h-768v352c0 19.2 12.8 32 32 32h704c19.2 0 32-12.8 32-32V518.4z"></path></svg>
			  	  	</span>
			  	  	<b style="font-weight: 300">2018年05月31日</b>&nbsp;&nbsp;
			  	  </div>
			  	  <div class="f_right" style="width: 25%">
					<span>
						<svg style="position: relative; bottom: -0.125em" width="14" height="14" t="1509598715318" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="3089" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M509.952 199.68c-267.776 0-501.76 219.136-501.76 326.656s232.96 326.656 501.248 326.656 501.248-219.136 501.248-326.656S778.24 199.68 509.952 199.68z m0 608.768c-263.68 0-457.216-217.088-457.216-282.112s193.536-282.112 457.216-282.112 457.216 217.088 457.216 282.112-196.096 282.112-457.216 282.112z" p-id="3090"></path><path d="M509.44 309.248c-119.808 0-216.576 97.28-216.064 217.088 0 119.808 97.28 216.576 217.088 216.064 119.808 0 216.576-97.28 216.064-217.088 0-119.296-96.768-216.064-216.064-216.064h-1.024z m0 365.568c-80.384 0-145.408-65.536-145.408-145.92s65.536-145.408 145.92-145.408 145.408 65.536 145.408 145.92-65.024 145.408-145.408 145.408h-0.512z" p-id="3091"></path></svg>
					</span><span>&nbsp;106</span>&nbsp;&nbsp;
					<span>
						<svg style="position: relative; bottom: -0.125em" width="14" height="14" t="1510555347486" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="1861" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M256.000712 398.249356C220.653727 398.249356 191.999822 427.354272 191.999822 463.271214 191.999822 499.193736 220.653727 528.300047 256.000712 528.300047 291.343424 528.300047 319.99733 499.193736 319.99733 463.271214 319.99733 427.354272 291.343424 398.249356 256.000712 398.249356L256.000712 398.249356 256.000712 398.249356ZM512.002849 398.249356C476.655863 398.249356 448.000534 427.354272 448.000534 463.271214 448.000534 499.193736 476.660136 528.300047 512.002849 528.300047 547.344137 528.300047 575.999466 499.193736 575.999466 463.271214 575.999466 427.354272 547.344137 398.249356 512.002849 398.249356L512.002849 398.249356 512.002849 398.249356ZM768.003562 398.249356C732.656574 398.249356 704.00267 427.354272 704.00267 463.271214 704.00267 499.193736 732.656574 528.300047 768.003562 528.300047 803.346271 528.300047 832.000176 499.193736 832.000176 463.271214 832.000176 427.354272 803.346271 398.249356 768.003562 398.249356L768.003562 398.249356 768.003562 398.249356ZM127.997507 73.142857C57.313507 73.142857 0 131.37501 0 203.193548L0 690.849809C0 762.673927 58.594009 828.873209 130.907481 828.873209L325.968258 828.873209C359.969221 864.347919 486.312565 990.610739 486.312565 990.610739 500.499343 1004.805435 522.99445 1004.477791 536.759928 989.742775 536.759928 989.742775 626.340718 892.625569 693.469508 828.873209L893.09252 828.873209C965.405989 828.873209 1024 762.668347 1024 690.849809L1024 203.193548C1024 131.37501 966.692191 73.142857 896.002494 73.142857L127.997507 73.142857 127.997507 73.142857ZM893.09252 764.433086 696.781152 764.433086C672.999992 764.433086 651.623156 788.383291 651.623156 788.383291L537.611356 905.884518C523.468162 920.460581 500.404798 920.008528 487.052412 905.884518L375.970511 788.383291C375.970511 788.383291 349.719506 764.433086 327.218848 764.433086L130.907481 764.433086C94.748608 764.433086 64.002315 726.755591 64.002315 690.849809L64.002315 203.193548C64.002315 167.276606 92.656219 138.164715 127.997507 138.164715L896.002494 138.164715C931.343777 138.164715 960.003387 167.276606 960.003387 203.193548L960.003387 690.849809C960.003387 726.755591 929.251394 764.433086 893.09252 764.433086L893.09252 764.433086Z" p-id="1862"></path></svg><span>&nbsp;4</span>&nbsp;&nbsp;
						<span>
							<svg style="position: relative; bottom: -0.125em" width="14" height="14" t="1521349270835" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="5429" xmlns:xlink="http://www.w3.org/1999/xlink"><path d="M987.733333 273.066667C947.2 151.466667 836.266667 64 704 64c-66.133333 0-128 23.466667-179.2 59.733333-8.533333 6.4-19.2 6.4-25.6 0C448 87.466667 386.133333 64 320 64 187.733333 64 74.666667 151.466667 36.266667 273.066667c-10.666667 21.333333-14.933333 53.333333-14.933334 93.866666 0 228.266667 339.2 497.066667 452.266667 580.266667 21.333333 17.066667 53.333333 17.066667 74.666667 0C663.466667 864 1002.666667 595.2 1002.666667 366.933333c0-42.666667-4.266667-72.533333-14.933334-93.866666z m-462.933333 640c-6.4 4.266667-17.066667 4.266667-23.466667 0C352 804.266667 64 556.8 64 366.933333v-2.133333c0-34.133333 4.266667-59.733333 10.666667-74.666667v-4.266666C110.933333 179.2 209.066667 106.666667 320 106.666667c61.866667 0 123.733333 25.6 170.666667 66.133333l8.533333 6.4c8.533333 6.4 19.2 6.4 27.733333 0l12.8-10.666667C584.533333 128 644.266667 106.666667 704 106.666667c110.933333 0 209.066667 72.533333 243.2 179.2v4.266666c6.4 17.066667 10.666667 42.666667 10.666667 76.8 2.133333 189.866667-285.866667 437.333333-433.066667 546.133334z m-192-366.933334C198.4 465.066667 213.333333 334.933333 213.333333 330.666667c2.133333-12.8-6.4-23.466667-17.066666-23.466667-10.666667-2.133333-23.466667 6.4-23.466667 19.2 0 6.4-21.333333 162.133333 138.666667 258.133333 4.266667 2.133333 6.4 2.133333 10.666666 2.133334 6.4 0 14.933333-4.266667 19.2-10.666667 4.266667-10.666667 0-23.466667-8.533333-29.866667z"></path></svg>
						</span><span>&nbsp;0</span>
					</span>
			  	  </div>
			  	</div>
			  </el-col>
		  	</el-row>
		    </el-main>
		    <el-aside width="358px" style="background-color: #fff; padding: 10px">
		    	<section>
		    		<img src="../assets/02.jpg" width="340" height="219">
		    		<section>
		    		  <h4>hock博客系统</h4>
		    		  <span>专注高端网站设计与开发！</span>
		    		  <div>
		    		  	<p>萨龙网络始建于2012年8月，是一家新生的优秀互联网综合服务提供商。</p>
					  	<p>公司坐落于美丽的大理洱海之滨，专注于高端网站建设、电子商务网站建设、客栈房间预订系统网站建设、移动互联应用、WordPress主题模板、服务器运维与网站托管，为企业客户的互联网应用提供一站式服务。</p>
		    		  </div>
		    		  	<a href="#">Read More</a>
		    		</section>
		    		
		    	</section>
		    </el-aside>
		  </el-container>
		  <el-footer>Footer</el-footer>
		</el-container>
	</div>
</template>

<script>
	export default {
	  data () {
	  	return {
	  	  activeIndex: '1',
	  	  slidefont: [
	  	  	{ text: '建立vue高品质生态圈', val:'专注前端开发100年' },
	  	  	{ text: 'hock博客系统', val:'萨龙网络原创简约新闻自媒体类 WordPress 主题，特色：用户中心、用户关注、 WooCommerce 商城、产品筛选与排序、付费阅读、付费查看视频、付费查看下载地址、HTML5音视频播放器、微信分享显示缩略图、点赞收藏、评论评分、打赏、站内信、百度推送、阿里云视频点播和优酷视频、认证作者加 V、前台编辑文章、关灯看视频、视频播放列表等自媒体实用的功能。' },
	  	  	{ text: 'JavaScript', val:'前端必备工具包之一' }
	  	  ],
	  	  artitle: [
	  	    {text: '多云模式并非完美的云生态',val: '多云是一种IT安排系统，它可以为企业客户的组织结合多个公共和私有云服务供应商。随着Azure，AWS，Google和本地云解决方案的业务遍及全球，多云模…'},
	  	    {text: '传统B2B如何转型跨境电商？',val: '电商回归到商业本质那就是产品本身，传统企业有产品研发实力和良好的供应链，如果能够很好解决这些挑战，相信跨境电商平台将是一个非常好的选择。顺势而为，跟时间…'},
	  	    {text: '首发丨极课大数据完成1亿元B轮融资，用AI提升学生作业、考试管',val: '极课大数据创立于2014年，致力于用AI提升学生作业、考试管理效率，团队规模300余人，技术人员占比2/3。截至目前，极课大数据已常态化部署1800多所…'},
	  	    {text: '易联云CEO王小名：如何打造一家盈利的供应链B2B服务平台',val: 'B2B的核心是建立资源共享服务平台，要整合生产商、经销商、终端店和物流商的优势资源，打造“技术、仓储、物流、金融、交易”五位一体的综合B2B服务平台，输…'},
	  	    {text: '百度：还在转身时',val: '互联网对于结果的兴趣远远高于过程，百度的自证难度也比腾讯和阿里高上许多，陷在泥潭里的滋味从来不曾好受，然而只有在彻底爬出来之后，它才能够重新构建公众的认…'},
	  	    {text: '内存的战争',val: '以前有人揭示过一个规律：很多产业，首先被美国人发明出来，美国人赚了一波钱后，产业基本上就在日本、韩国、大陆、台湾这四个地方转圈。'}
	  	  ]
	  	}
	  },
	  methods: {
        handleSelect(key, keyPath) {
        console.log(key, keyPath);
        }
	  }
	}
</script>

<style lang="scss">
  @media (max-width: 1200px) {
	.w-1272 {
		display: none;
	}
	#w_1272 {
		display: block;
	}
	#searchIcon {
		display: none;
	}
	#carousels {
  		width: 100%;
  	}
  }
  #contain {
	.el-container {
	  .el-header {
	  	padding: 0 10px;
		background-color: #fff;
		  .w-1272 {
			width: 1200px;
			height: inherit;
			margin: 0 auto;
			.el-col {
			  .wechatsearch {
			  	height: 76px;
			  	line-height: 76px;
			  	margin-bottom: 0;
			  	li {
			  		float: right;
			  		padding: 0 10px;
			  		a {
			  			display: inline-block;
			  			svg {
			  				position: relative;
			  				bottom: -0.525em;
			  				fill: #999;
			  				&:hover {
			  					fill: #2C74E6;
			  				}
			  			}
			  		}
			  	}
			  }
			  .el-menu {
			  	border: none;
			  }
			}
		  }
		  .w_1272 {
			width: 100%; // 此处注意优先级的问题, style > id > class
			height: inherit;
			.el-col {
			  height: 76px;
			  line-height: 76px;
			  a {
			  	img {
			  		height: inherit;
			  		display: inline-block;
			  	}
			  }
			}
		  }
	  }
	  .carousels {
	  	width: 77%;
	  	margin: 0 auto;
	  	margin-top: 25px;
	  }
	}
  }
  .w_1272 {
  	display: none;
  }
  // 圣杯布局样式-- < 1200 布局
  #wrap{ width: 100%; height: 76px; float: left;}
  #wrap #center{ margin: 0 50px; height: 76px;}
  #left,#right{ float: left; width: 50px; height: 76px;}
  #left {margin-left: -100%;}
  #right{margin-left: -50px;}

  .el-carousel__item h3 {
    color: #475669;
    font-size: 18px;
    opacity: 0.75;
    line-height: 300px;
    margin: 0;
  }
</style>