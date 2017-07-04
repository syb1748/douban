<template>
	<div class="box2">
		<slot name='tupian5'></slot>
		<div class="box1">
			<span class="tixing">提醒</span>
			<span class="t1">暂无新提醒</span>			
		</div>
		<div class="box3">
			<div class="top1">
				<div class="item1">
					<img src="../assets/images/ic_photo_liked.png"><br/>
					<span>喜欢</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_movies_tvs.png"><br/>
					<span>日记</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_note.png"><br/>
					<span>相册</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_status.png"><br/>
					<span>我的广播</span>
				</div>
			</div>
			<div class="mid2">
				<div class="item1">
					<img src="../assets/images/ic_photo_liked.png"><br/>
					<span>喜欢</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_movies_tvs.png"><br/>
					<span>日记</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_note.png"><br/>
					<span>相册</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_status.png"><br/>
					<span>我的广播</span>
				</div>
			</div>
			<div class="footer1">
				<div class="item1">
					<img src="../assets/images/ic_photo_liked.png"><br/>
					<span>喜欢</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_movies_tvs.png"><br/>
					<span>日记</span>
				</div>
				<div class="item1">
					<img src="../assets/images/ic_my_note.png"><br/>
					<span>相册</span>
				</div>
			</div>
		</div>
	</div>
</template>
<style type="text/css">
	.box2{ width: 100%; background-color: #f2f1ee;  height: 2000px; }
	.tu6{ width: 100%; }
	.box1{ width: 100%; height: 100px; background-color: #fff;}
	.tixing{ border-bottom: 1px solid #ccc; font-size: 20px; padding: 5px 10px;}
	.t1{ color: #ccc; font-size: 14px; position: absolute;  left: 100px; top: 250px; }
	.box3{ width: 100%; height: 300px; background-color: #fff; margin-top: 20px;}
	.top1{ border-bottom: 1px solid #eee; padding-bottom: 30px; width: 100%; height: 60px}
	.mid2{ border-bottom: 1px solid #eee; padding-bottom: 30px; width: 100%; height: 60px}
	.item1{ width: 25%; text-align: center; padding-top: 30px; float: left}
	.footer1{ padding-bottom: 30px; width: 100%; height: 60px}
</style>