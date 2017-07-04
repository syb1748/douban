<template>
	<div>
		<MyHeader>
			<span class='title'>小组</span>
			<img src="../../assets/images/ic_group_search.png" class="search1" slot='left2'>
			<img src="../../assets/images/ic_create_group_chat_blue.png" class="chat1" slot='right2'>
		</MyHeader>
		<G1>
			<img src="../../assets/images/images/m1_99.jpg" slot='tupian2' class="tu3">
			<img src="../../assets/images/images/m_100_07.jpg" slot='tupian3' class="tu4">
			<img src="../../assets/images/images/p42157700.jpg" slot='tupian4' class="tu5">
		</G1>
	</div>
</template>
<script>
	import MyHeader from '../../components/header'
	import G1 from '../../components/g1'
	export default{
		components:{
			MyHeader,
			G1
		}
	}
</script>
