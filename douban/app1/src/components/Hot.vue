<template>
	<div class="re">
		<slot name='tupian'></slot>
		<h1>热点</h1>
		<slot name='title1'></slot>
		<p>只需要三四个小时就可以产生出一篇完全<br/>可以骗过查重系统的论文</p>
		<p class="zuozhe">作者：土豆公社</p>
	</div>
</template>
<style type="text/css">
	.re{ position: absolute; left: 0; top: 148px; background-color: #fff;  width: 100%; height: 220px;border-bottom: 1px solid #ccc;}
	h1{ color: #e1a26c; padding-left: 10px; }
	h2{ font-size: 20px; padding-left: 10px;}
	p{ color: #b6b6b6; font-size: 12px; padding-top: 15px; padding-left: 10px;}
	.zuozhe{ padding-top: 10px; }
	.tu1{ width: 100px;  height: 120px; position: absolute; left: 254px; top: 50px; }
</style>