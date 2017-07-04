<template>
	<div class="beijing">
		<slot name='tupian2'></slot>
		<h3>发现有趣的人</h3>
		<span class="guan">关注他们。发现更大的世界</span>
		<div class="box">
			<h4>陆大鹏HANS</h4>
			<slot name='tupian3'></slot>
			<button>关注</button>
			<p>版权归作者所有，任何形式转载请联系作者。
				作者：UnderstandA（来自豆瓣）
				来源：https://www.douban.com/note/616949394/

他说。
爱或者恨一座城市，到何种程度，会让他说：应当从各处放火把这个城市给烧了才好。

于是理解了为什么他临终前要求好友将他所有的作品付诸一炬，
他最担心的事情还是发生了，而且继续发生着：
这世界依然荒谬，曾经反思着荒谬的他，现在也成为了荒谬的一部分。
人们消费着他的忧郁和痛苦。
他是宁可人们秘密地默默地看他的小说的，而不是如此被消费。
布拉格这座城这座牢笼，依然关着卡夫卡。</p>
		<slot name='tupian4'></slot>
		</div>
	</div>
</template>
<style type="text/css">
	.beijing{ width: 100%; height: 2000px; background-color: #f2f1ee; }
	h3{ padding-left: 150px; position: absolute; left:0; top: 80px; padding-bottom: 20px;}
	.guan{ padding-left: 150px; color: #9b9b9b; font-size: 12px; position: absolute; left: 0; top: 110px;}
	.tu3{ width: 20%; padding-left: 50px;}
	.box{ width: 80%; background-color: #fff; height: 800px; position: absolute; left: 40px; top: 130px; }
	h4{ padding-left: 60px; padding-top: 20px; position: absolute; left: 0; top: 0;}
	.tu4{ width: 10%; padding-left: 10px; padding-top:10px; }
	button{ padding:5px 10px; border-radius: 4px; background-color:lightgreen; border: none; color: #fff; margin-left: 180px;}
	.tu5{ width: 100%;}
</style> 