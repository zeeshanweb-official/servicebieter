<template>
    <div>
         <div class="sliderChanged">
            <div class="row ">
                <carousel  :items=3 :autoplayTimeout=4000 :nav='false' :autowidth='false' :smartSpeed=900 :loop='true' :autoplay='true' :dots='false' :slideBy=3>
                    <div class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?1">
                        <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>
                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?2">
                        <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>
                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?3">
                         <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>

                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?4">
                         <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>
                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?1">
                         <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>
                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?2">
                         <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>
                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?3">
                         <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>
                    <div  class="itemsofslider">
                        <img src="https://placeimg.com/200/200/any?4">
                         <div class="overlay" id="overlay">
                            <p>
                            Logo Design
                            </p>
                        </div>
                    </div>

            </carousel>
            </div>
            </div>
    </div>
</template>
<script>

import carousel from 'vue-owl-carousel'
export default {
     components: { carousel },
}
</script>
<style>
    
.itemsofslider:hover #overlay {
 display: block;
 
}
.overlay>p{
    margin-top: 40%;
    font-weight: 900;
}
.overlay{
    background-color: #000;
    opacity: 0.5;
    position: absolute;
    top: 0%;
    width: 100%;
    height: 100%;
    color:white;
    text-align: center;
    font-size: 30px;
    display: none;
}
.sliderChanged{
    width: 93%;
    margin: 20px 35px;
    overflow: hidden;
}
</style>