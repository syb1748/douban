<template>
	<div>
		{{msg}}
		<Parent></Parent>
	</div>
</template>
<script>
import Parent from '../components/Parent'
	export default{
		name:'Index',
		data:function(){
			return{
				msg:'hello'
			}
		},
		components:{
			Parent
		}
	}
</script>