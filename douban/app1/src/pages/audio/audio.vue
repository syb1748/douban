<template>
	<div>
		<MyHeader>
			<span class='title'>书影音</span>
			<img src="../../assets/images/ic_group_search.png" class="search1" slot='left1'>
			<img src="../../assets/images/ic_create_group_chat_blue.png" class="chat1" slot='right1'>
		</MyHeader>
			<ul>
				<li><router-link to='/audio/film'>电影</router-link></li>
				<li><router-link to='/audio/book'>读书</router-link></li>
				<li><router-link to='/audio/film'>电影</router-link></li>
				<li><router-link to='/audio/book'>读书</router-link></li>
		<router-view></router-view>
			</ul>
	</div>
</template>
<script>
	import MyHeader from '../../components/header'
	export default{
		components:{
			MyHeader
		}
	}
</script>
<style>
	ul{ width:100%; background-color:#fff; height: 40px; position: absolute; left: 0; top: 40px;}
	li{ display:inline-block; text-decoration: none; list-style: none; line-height: 40px;}
	a{ text-decoration: none; padding:5px 20px; color: #000;}
</style>