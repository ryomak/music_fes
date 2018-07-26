<template>
	<div class="place">
		<section>
				<h2><span>Place</span></h2>
			<div class="innerS">
				<ul class="col2">
					<li>
						<p>〒530-0012 <br>大阪府大阪市北区芝田１丁目１</p>
						<p>営業時間 10:00〜20:00（水曜定休）</p>
						<p>※都合により休業する場合がございます</p>
						<p id="sns">
							<a href="#" target="_blank"><img src="@/assets/iconFb.png" width="20" height="20" alt="FB"></a>
							<a href="#" target="_blank"><img src="@/assets/iconTw.png" width="20" height="20" alt="twitter"></a>
							<a href="#" target="_blank"><img src="@/assets/iconInsta.png" width="20" height="20" alt="Instagram"></a>
							<a href="#" target="_blank"><img src="@/assets/iconYouTube.png" width="20" height="20" alt="You Tube"></a>
						</p>
					</li>
					<li>
						<div id="map">
							<!-- GOOGLE MAP -->
							<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3280.006060490924!2d135.4962382147425!3d34.70502708043336!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6000e6918dc9e10d%3A0x47b718217281e2c3!2z5qKF55Sw6aeF!5e0!3m2!1sja!2sjp!4v1532600153734" allowfullscreen></iframe>
							<!-- // GOOGLE MAP -->
						</div>
					</li>
				</ul>
			</div>
		</section>
	</div>
</template>
<script>
	export default{
		name:"Place"
	}
	
</script>
<style scoped>
	.place p{
	margin-bottom: 5px;
}

.col2 li{
	display: inline-block;
	width: 100%;
	margin: 20px 0;
}

#sns img{
	padding: 35px 10px 5px 0;
}

#sns a:hover img{
	opacity: .8;
}

#map{
	position: relative;
	padding-bottom: 75%;
	height: 0;
	overflow: hidden;
	z-index: 0;
}

#map iframe{
	position: absolute;
	top: 0;
	left: 0;
	width: 100% !important;
	height: 100% !important;
	border: 0;
}
</style>>