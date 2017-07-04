<template>
	<div class='t'>
		<Wrap :sel='selected'>
			<item txt='首页' id='home' @change='getval'>
				<img src='../assets/images/ic_tab_home_active.png' slot='active' class='icon'>
				<img src='../assets/images/ic_tab_home_normal.png' slot='normal' class='icon'>
			</item>
			<item txt='书影音' id='audio' @change='getval'>
				<img src='../assets/images/ic_tab_home_active.png' slot='active' class='icon'>
				<img src='../assets/images/ic_tab_home_normal.png' slot='normal' class='icon'>
			</item>
			<item txt='小组' id='group' @change='getval'>
				<img src='../assets/images/ic_tab_group_active.png' slot='active' class='icon'>
				<img src='../assets/images/ic_tab_group_normal.png' slot='normal' class='icon'>
			</item>
			<item txt='讨论' id='broadcast' @change='getval'>
				<img src='../assets/images/ic_tab_home_active.png' slot='active' class='icon'>
				<img src='../assets/images/ic_tab_home_normal.png' slot='normal' class='icon'>
			</item>
			<item txt='我的' id='mine' @change='getval'>
				<img src='../assets/images/ic_tab_home_active.png' slot='active' class='icon'>
				<img src='../assets/images/ic_tab_home_normal.png' slot='normal' class='icon'>
			</item>
		</Wrap>
	</div>
</template>
<script>
	import Wrap from './Wrap'
	import Item from './Item'
	export default{
		components:{
		Wrap:Wrap,
		Item:Item
		},
		data:function(){
			return{
			selected:'Home'
			}
		},
		methods:{
			getval:function(val){
				this.selected=val
			}
		}
	}
</script>
<style>

</style>
