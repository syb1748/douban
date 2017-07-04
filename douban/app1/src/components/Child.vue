<template>
	<div>
		<ul>
			<li @click='turnPages(1)'><a href=''>首页</a></li>
			<li @click='turnPages(pages-1)'><a href=''>下一页</a></li>
			<li v-if='pages-3>0' @click='turnPages(pages-3)'><a href='#'v-text='pages-3'></a></li>
			<li v-if='pages-2>0' @click='turnPages(pages-2)'><a href='#' v-text='pages-2'></a></li>
			<li v-if='pages-1>0' @click='turnPages(pages-1)'><a href='#' v-text='pages-1'></a></li>
			<li class='ac'><a href='' v-text='pages'>4</a></li>
			<li v-if='pages+1<total' @click='turnPages(pages+1)'><a href='#' v-text='pages+1' ></a></li>
			<li v-if='pages+2<total' @click='turnPages(pages+2)'><a href='#' v-text='pages+2'></a></li>
			<li v-if='pages+3<total' @click='turnPages(pages+3)'><a href='#' v-text='pages+3'></a></li>
			<li v-if='pages+4<total' @click='turnPages(pages+4)'><a href='#' v-text='pages+4'></a></li>
			<li @click='turnPages(pages+1)'><a href='#' @click='turnpages(pages+1)'>下一页</a></li>
			<li @click='turnPages(total)'><a href='#' @click='turnpages(total)'>末页</a></li>
		</ul>
		<small><span>当前页数{{pages}}</span><span>最大页数{{total}}</span></small>
		<input type='number' v-model='pageGo' :class='{err:bol}'><button @click='turnPages(pageGo)'>GO</button></input>
	</div>
</template>
<script>
	export default{
		data:function(){
			return{
				pages:100,
				total:100,
				pageGo:'',
				bol:false
			}
		},
			methods:{
				turnPages:function(num){
					this.pages=num
					if(num<1 || num>100 || !num){
						this.bol=true
						return
					}else{
						this.bol=false
					}
				}
			}		
	}
</script>
<style>
	ul{display:inline-block; margin:auto}
	ul li{list-style:none; padding:5px 10px; border:solid 1px gray; float:left; height:30px; line-height:30px;}
	a{ text-decoration:none;}
	.ac{ background-color:skyblue}
	.err{ border:solid 1px red}
	.disabled{}
</style>