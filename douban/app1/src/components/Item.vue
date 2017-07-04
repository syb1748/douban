<template>
	<div class='i' @click='fn'>
		<span v-show='bol'><slot name='normal'></slot><br/></span>
		<span v-show='!bol'><slot name='active'></slot><br/></span>
		<span v-text='txt'></span>
	</div>
</template>
<script>
	export default{
		props:['txt','id'],
	computed:{
		bol:function(){
			if(this.$parent.sel==this.id){
				return false
			}
			return true
		},
	},
	methods:{
		fn:function(){
			this.$router.push('/'+this.id),

			this.$emit('change',this.id)
		}
	}
	}
</script>
<style>
	.i{ width:20%; float:left; text-align: center;}
	span{ font-size: 16px; }
	.icon{ width:33px;}
</style>