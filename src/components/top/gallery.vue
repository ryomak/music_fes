<template>
	<div class="gallery">
		<section>
				<h2><span>Gallery</span></h2>
			<div class="innerS te">
				イベントで撮った写真をここにあげていきます．
			</div>
			<ul class="img">
				<li><img src="@/assets/photo01.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo02.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo03.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo04.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo05.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo06.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo07.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo08.jpg" width="426" height="418" alt=""></li>
				<li><img src="@/assets/photo09.jpg" width="426" height="418" alt=""></li>
			</ul>
		</section>
	</div>
</template>
<script>
	export default{
		name:"Gallery"
	}
	
</script>
<style>
.gallery{
	padding: 0 !important;
}

.gallery header{
	display: none;
}

.img li{
	float: left;
	width: calc(100%/3);
	line-height: 0;
}

.img img{
	width: 100%;
	height: auto;
}

.te{
	text-align: center;
}
</style> 