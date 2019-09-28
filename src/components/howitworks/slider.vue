<template>
<div class="container-fluid mb-5 mx-0 px-0">
	<agile :dots="false" :slidesToShow=3 :infinite="true" :autoplay='true' ref="carousel" :navButtons='false' :autoplay-speed="5000">
		<div class="slide">
				<div class="image-container">
					<img src="https://placeimg.com/300/200/any?1" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		<div class="slide">
			<div class="image-container">
					<img src="https://placeimg.com/300/200/any?2" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		<div class="slide">
			<div class="image-container">
					<img src="https://placeimg.com/300/200/any?3" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		<div class="slide">
			<div class="image-container">
					<img src="https://placeimg.com/300/200/any?4" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		
		<div class="slide">
			<div class="image-container">
					<img src="https://placeimg.com/300/200/any?1" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		<div class="slide">
			<div class="image-container">
					<img src="https://placeimg.com/300/200/any?2" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		<div class="slide">
				<div class="image-container">
					<img src="https://placeimg.com/300/200/any?3" />
					<div class="image-caption">
					<h1>LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
		<div class="slide">
			<div class="image-container">
					<img src="https://placeimg.com/300/200/any?4" />
					<div class="image-caption">
					<h1 class="headon">LOGO Design</h1>
					<p>Branding</p>
					<div class="littleline"></div>
					<div class="dets"><p>More Details<i class="fa fa-caret-right" aria-hidden="true"></i></p></div>
					</div>
				</div>
		</div>
	</agile>
 <!-- <carousel :nav='false' :autoplay='true' >
				
 </carousel> -->
<div class="prev1">
	<span @click="$refs.carousel.goToPrev()" class="fa-stack fa-lg" id="prev" style="font-size:20px; margin-left:10px; margin-top:120px; color: #9a9595; cursor:pointer">
  <i class="fa fa-angle-left fa-stack-1x"  style="font-size:40px; margin-left:-2px;"></i>
  <i class="fa fa-circle-thin fa-stack-2x"></i>
</span>
</div>
<div class="next1">
	<span @click="$refs.carousel.goToNext()" class="fa-stack fa-lg" id="next" style="font-size:20px; margin-top:120px; margin-left:10px; color: #9a9595; cursor:pointer">
  <i class="fa fa-angle-right fa-stack-1x" style="font-size:40px; margin-left:2px;"></i>
  <i class="fa fa-circle-thin fa-stack-2x "></i>
</span>
	<!-- <i class="fa fa-arrow-circle-right" style="font-size:40px; margin-top:120px; color: white; cursor:pointer"	></i> -->
</div>
</div>
</template>

<script>
import $ from 'jquery' 
window.$ = $;
import { VueAgile } from 'vue-agile'

  export default {
    name: 'App',
    components: {
	 agile: VueAgile
	},
}
</script>
<style>
.agile__slide{
	border: 5px solid white;
}
.owl-prev{
	position: fixed;
	left: 0px;
	bottom: 100px;
}
.owl-item{
	border:5px solid white;
}
.prev1,.next1{
	position: absolute;
	width: 60px;
	height: 295px;
	background-color: rgb(60, 60, 60);
	bottom: 105px;
	opacity: 0.9;
	z-index: 1;
}
.next1{
	right: 0px;
}


.headon {
  text-align: center;
  font-family: 'Indie Flower', cursive;
  color: #00bfb6;
  text-decoration: underline;
}

.image-container {
  float: left;
  width: 445px;
  height: 295px;
  position: relative;
  cursor: pointer;
}

.image-container img {
  width: 445px;
  height: 295px;
  position: absolute;
}

.image-caption {
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.7);
  position: absolute;
  opacity: 0;
  transition: all 300ms ease-in-out;
  -webkit-transition: all 300ms ease-in-out;
  -moz-transition: all 300ms ease-in-out;
  -o-transition: all 300ms ease-in-out;
  -ms-transition: all 300ms ease-in-out;
}

.image-caption h1 {
  padding: 45px 0px 5px 0px;
  text-align: center;
  margin-left: -15px;
  text-transform: uppercase;
  font-family: 'Indie Flower', cursive;
  font-size: 25px;
  color: #00bfb6;
}

.image-caption p {
  text-align: center;
  font-family: 'Overpass Mono', monospace;
  color: #fff;
}

.image-container:hover .image-caption {
  opacity: 1;
}


/* media queries */

@media all and (min-width: 0px) and (max-width: 520px) {
  #wrapper {
    width: 100%;
    height: 100%;
    padding: 0px 70px
  }
}

@media all and (min-width: 521px) and (max-width: 700px) {
  #wrapper {
    width: 100%;
    height: 100%;
  }
  .image-container {
    float: left;
    width: 48%;
    margin: 5px;
    overflow: hidden;
    position: relative;
  }
  .image-caption {
    width: 250px;
    height: 200px;
  }
}
</style>