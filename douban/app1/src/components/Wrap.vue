<template>
	<div class='wrap'>
		<slot></slot>
	</div>
</template>
<script>
export default{
	props:['sel']
}
</script>
<style>
	.wrap{ height:64px; width:100%; background-color:#ccc; position:fixed; left:0; bottom:0; padding-top:7px; text-align: center;}
</style>