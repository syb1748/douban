<template>
	<div class='h' :style='{background:col}'>
		<slot></slot>
		<slot name='left'></slot>
		<slot name='right'></slot>
		<slot name='left1'></slot>
		<slot name='right1'></slot>
		<slot name='left2'></slot>
		<slot name='right2'></slot>
		<slot name='right3'></slot>
		<slot name='left3'></slot>
		<slot name='right4'></slot>		
	</div>
</template>
<script>
	export default {
		props:{
			col:{
				default:'#f7f7f7'
			}
		}
	}
</script>
<style>
	.h{ width:100%; height:48px; background-color:green; position:fixed; left:0; top:0}
	.title{ color:black; font-size:16px; height:48px; line-height:48px; text-align: center; position: absolute; left: 160px; top: 0;}
	input{ border: none; border-radius: 8px; height: 25px; width: 80%; position: absolute; top: 12px; left: 20px; text-indent: 3em}
	img{ width: 20px;}
	.search{ left: 23px; top: 16px; position: absolute; }
	.scan{ left: 280px; top: 16px ; position: absolute;}
	.chat{ left: 340px; top:16px ; position: absolute;}
	.banner{ height: 100px; width: 100%; position: fixed; left: 0; top: 48px; }
	.search1{ position: absolute; left: 310px; top: 16px; }
	.chat1{ position: absolute; left: 340px; top: 16px; }
</style>