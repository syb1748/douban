<template>
	<div>
		<MyHeader col='#42c055'>
			<input type="text" name='' placeholder="图书广播 书影音">
			<img src="../../assets/images/ic_search_gray.png" slot='left' class="search" >
			<img src="../../assets/images/ic_scan_gray.png" slot='right'  class="scan">
			</input>
			<img src="../../assets/images/ic_chat_white.png" class="chat">
		</MyHeader>
		<div class="banner">
			
		</div>
		<MyHot v-for="item in arr">
			<h2 slot='title1'>{{item.title}}</h2>
			<img src="../../assets/images/m1_03.jpg" slot='tupian' class="tu1">
		</MyHot>
		<HotItem v-for="item in arr">
			<h2 slot='title2'>{{item.title}}</h2>
			<img src="../../assets/images/m1_03.jpg" slot='tupian1' class="tu2">
		</HotItem>
		<Banner swipeid='swipe01'>
			<div class="swiper-slide" slot='swiper-con'><img src="../../assets/images/banner/01.jpg"></div>
			<div class="swiper-slide" slot='swiper-con'><img src="../../assets/images/banner/02.jpg"></div>
			<div class="swiper-slide" slot='swiper-con'><img src="../../assets/images/banner/03.jpg"></div>
		</Banner>
	</div>
</template>
<script>
	import MyHeader from '../../components/header'
	import MyHot from '../../components/Hot'
	import HotItem from '../../components/HotItem'
	import Banner from '../../components/swiper'
	export default{
		components:{
			MyHeader:MyHeader,
			MyHot:MyHot,
			HotItem:HotItem,
			Banner:Banner
		},
		mounted:function(){
			this.search()
		},
		methods:{
			search:function(){
				console.log(this.search)
				this.axios.get('/api/homeData').then((response) => {
		          	console.log(response.data.data.recommend_feeds);
		          	this.arr = response.data.data.recommend_feeds;
		        })				
			}
		},
		data:function(){
			return{
				arr:[]
			}
		}

	}
</script>