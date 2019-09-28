<template>
<div>
<div class="scrollbar style-3">
<div class="row overflow-hidden mx-0">
      <div class="col-md-3  pr-0 ad">
        <div class="scrollbar style-3 py-3">
            <companySideLine></companySideLine>
        </div>
      </div>
      <div class="col-md-7 px-1 py-3">
        <div class="scrollbar style-3">
        <div class="container px-2">
      

      <div class="card cardslider">
        <div class="card-body p-1">
           
            <div class="slider">
             
              <div>
                <div class="carousel">
                  <ul class="slides">
                    <div class="overlay"></div>
                    <input type="radio" name="radio-buttons" id="img-1" checked />
                    <li class="slide-container">

                      <div class="slide-image">
                        <p class="item-1">This is your last chance. After this, there is no turning back.</p>
                        <img
                          src="https://upload.wikimedia.org/wikipedia/commons/9/9e/Timisoara_-_Regional_Business_Centre.jpg">
                      </div>
                      <div class="carousel-controls">

                        <label for="img-3" class="prev-slide">
                          <span>&lsaquo;</span>
                        </label>
                        <label for="img-2" class="next-slide">
                          <span>&rsaquo;</span>
                        </label>
                      </div>
                    </li>
                    <input type="radio" name="radio-buttons" id="img-2" />
                    <li class="slide-container">
                      <div class="slide-image">
                        <p class="item-1">This is your last chance. After this, there is no turning back.</p>
                        <img src="http://www.timisoaranight.gruzphoto.eu/IMG_8554.jpg">
                      </div>
                      <div class="carousel-controls">
                        <label for="img-1" class="prev-slide">
                          <span>&lsaquo;</span>
                        </label>
                        <label for="img-3" class="next-slide">
                          <span>&rsaquo;</span>
                        </label>
                      </div>
                    </li>
                    <input type="radio" name="radio-buttons" id="img-3" />
                    <li class="slide-container">
                      <div class="slide-image">
                        <p class="item-1">This is your last chance. After this, there is no turning back.</p>
                        <img src="https://speakzeasy.files.wordpress.com/2015/05/twa_blogpic_timisoara-4415.jpg">
                      </div>
                      <div class="carousel-controls">
                        <label for="img-2" class="prev-slide">
                          <span>&lsaquo;</span>
                        </label>
                        <label for="img-1" class="next-slide">
                          <span>&rsaquo;</span>
                        </label>
                      </div>
                    </li>
                    <div class="carousel-dots">
                      <label for="img-1" class="carousel-dot" id="img-dot-1"></label>
                      <label for="img-2" class="carousel-dot" id="img-dot-2"></label>
                      <label for="img-3" class="carousel-dot" id="img-dot-3"></label>
                    </div>
                  </ul>
                </div>
              </div>

            </div>
        </div> 


        <div class="second">
          What I am Looking For?
        </div>
        <div class="third">
          <p class="first-paragraph">100% Result Till now with 5/5 rating with Preferred Freelancer chosen by Freelancer itself..
          </p>
         <div class="second-paragraph">
            <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Inventore cum voluptates provident cupiditate illum, consequatur, doloremque reprehenderit ratione voluptatum hic recusandae nihil molestias necessitatibus velit enim deleniti. Natus, laudantium distinctio adipisci hic delectus velit provident minus ea harum laboriosam sint.
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ad rerum earum, corporis odio sunt placeat voluptatum nulla commodi cum, aliquid architecto libero incidunt dicta provident dolor nihil consequuntur, molestiae culpa hic ea. Assumenda et voluptatem dicta, earum doloribus ab! Cum dolor molestias quis iste, ad explicabo optio consectetur eum voluptate.
          </p>
         </div>
        </div>
        <div class="forth">
          <div class="row">
            <div class="col-md-6">
              <div class="one">
                  Job Features & Overviews
              </div>
              <div class="two">
                <ul class="customlist">
                  <li v-for="item in overviews" :key="item.index">{{item}}</li>
                </ul>
              </div>
            </div>
            <div class="col-md-6">
              <div class="one">
                  Experience Requirements
              </div>
              <div class="two">
                <ul class="customlist">
                  <li v-for="item in experiences" :key="item.index">{{item}}</li>
                </ul>
              </div>
            </div>
          </div>
        </div>
    <div class="container">
       <div class="row">
    <div class="col sbox">
      <div class="pak">
        <h2>
          <i class="fa fa-star-half-o"></i>
          Feedback
        </h2>
          <div class="data">
              <ul class="review-star px-0"><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i><i class="fa fa-star"></i>
                <i class="fa fa-star"></i>
              </ul>
            </div>
      </div>
    </div>
    <div class="col sbox">
      <div class="pak">
        <h2>
          <i class="fa fa-shopping-cart"></i>
          Sales
        </h2>
          <div class="data">
              <p class="price">4005</p>
            </div>
      </div>
    </div>  <div class="col sbox">
      <div class="pak" style="height: 98px;">
        <h2>
          <i class="fa fa-euro"></i>
          Price
        </h2>
          <div class="data">
              <p class="price">500,4</p>
             <p></p>
            </div>
      </div>
    </div>  <div class="col sbox">
      <div class="pak">
        <h2>
          <i class="fa fa-shopping-bag"></i>
          Buy
        </h2>
          <div class="data">
              <div class="btn btn-sm btn-arang">Buy</div>
            </div>
      </div>
    </div>
  </div>
    </div>
    <div class="sharediv">
          <h3><i class="fa fa-share-alt"></i> Share</h3>
    </div>
    <div class="sharediv2">
          <h3>
            <ul class="newdiv">
                      <li><a href="service-title.html#"><i class="fa fa-facebook"></i></a></li>
                      <li><a href="service-title.html#"><i class="fa fa-google-plus"></i></a></li>
                      <li><a href="service-title.html#"><i class="fa fa-twitter"></i></a></li>
                    </ul>
          </h3>
    </div>
    <hr>
<div class="related-ads">
  <div class="title3">
    <h3>
      Other Services From This Company
    </h3>
      
  </div>
  <otherServices></otherServices>
</div>
<div class="title3 title4">
   <h3>
     Service Feedback
    </h3>
</div>
<appcomments></appcomments>
</div>
  </div>
      </div>
      </div>
      <div class="col-md-3 pr-0 ad">
          <div class="scrollbar style-3 py-3">
          <appAd v-for="ad in ads" :key="ad.index" :ad="ad"></appAd>
          <div class="card shani">
            <p class="text-center" style="font-size:21px;">Our Services</p>
             <appServices  class="col-sm-12 p-0" v-for="image in images" :key="image.index" :image="image.image"></appServices>
          </div>
          </div>
      </div>
  </div>
</div>

  <div class="modal" id="myModal">
    <div class="modal-dialog">
      <div class="modal-content">
      
        <!-- Modal Header -->
        <div class="modal-header">
          <h4 class="modal-title">Modal Heading</h4>
          <button type="button" class="close" data-dismiss="modal">&times;</button>
        </div>
        
        <!-- Modal body -->
        <div class="modal-body">
          Modal body..
        </div>
        
        <!-- Modal footer -->
        <div class="modal-footer">
          <button type="button" class="btn btn-danger" data-dismiss="modal">Close</button>
        </div>
        
      </div>
    </div>
  </div>
  
</div>

</template>
<script>
import ad from '../../BeMember/ad'
import services from '../myservice'
import companySideLine from './companyside'
import otherServices from './otherservices'
import appcomments from './comments'
export default {
    data() {
      return {
          experiences:[
            'PSD TO HTML5 ( Elite author in themeforest)',
            'Great experience with Linux, Server Optimizing, Failover Clustering, Security, Virtualization know common used utilites, scripts and services such as Apache, PHP, MySQL, Nginx and many others.',
            'Donec venenatis ante a imperdiet maximus. Sed in justo porta, rutrum velit non, blandit lorem.',
            
          ],
          overviews:[
            'wordpress expert',
            'Opencart listed Partner', 
            'Magento Certified', 
            'Php Larvel ,Zend Framework', 
            'Certified Social Engine', 
            'Prestashop , CS cart and Drupal, ZenCart developer', 
          ],
         images:[
                  {
                    image:'01.jpg'
                  },
                  {
                    image:'02.jpg'
                  },
                  {
                    image:'03.jpg'
                  },
                  {
                    image:'04.jpg'
                  },
                  {
                    image:'05.jpg'
                  },
                  {
                    image:'06.jpg'
                  },
                  {
                    image:'07.jpg'
                  },
                  {
                    image:'08.jpg'
                  },
                ],
        ads:[
                  {
                      title:'Professional',
                      type:'image',
                      img_src:'@/assets/images/SmartStaff-Logo-Rohan-02_1.png',
                      text_muted:'What is SmartStaff'
                    },
                  {
                      title:'Secure',
                      type:'Icon',
                      className:'fa fa-shield',
                      text_muted:'100% secure',
                      text_muted2:'Job is Done or money back'
                    },
                ]
      }
    },
    components:{
        appAd:ad,
        companySideLine,
        appServices:services,
        otherServices,
        appcomments,
    },
     methods: { 
           scrollToTop() {
                window.scrollTo(0,0);
           }
        }
    
}
</script>



<style scoped>
.title3{
background-color: #ededed;
}
.title3 > h3{
text-align: center;
padding: 15px 0px;
font-size: 24px;
font-family: 'Raleway', Arial, Helvetica, sans-serif;
font-weight: 500;
line-height: 26.4px;
margin-bottom: 15px;
}
.title4{
  margin-left: 10px;
  width: 97%;
}
.title4 > h3{
text-align: center;
padding: 5px 0px;
font-size: 24px;
font-family: 'Raleway', Arial, Helvetica, sans-serif;
font-weight: 500;
line-height: 26.4px;
margin-bottom: 10px;
margin-left: 10px;
}
.sharediv{
  text-align: center;
  border: 1px solid #ededed;
  padding: 10px 0px;
  font-family: 'Raleway', Arial, Helvetica, sans-serif;
  margin-left: 9px;
  margin-top: 10px;
      width: 97%;
}
.sharediv2{
  text-align: center;
  border: 1px solid #ededed;
  padding: 10px 0px;
  font-family: 'Raleway', Arial, Helvetica, sans-serif;
  margin-left: 9px;
  border-top: none;
  width: 97%;
}
.sharediv2 > ul {
    float: left;
    margin: 0 auto;
    padding: 20px 0;
    width: 100%;
}
.newdiv{
  padding: 0%;
}
.newdiv > li{
    list-style: none;
    display: inline-block;
    margin: 2px;
    font-size: 14px;
}
.sharediv2 a i {
    line-height: 35px;
}
.sharediv2 a {
    border: 1px solid #414141;
    color: #414141;
    display: inline-block;
    height: 35px;
    transition: all 0.3s ease 0s;
    width: 35px;
}
.sharediv2 a:hover {
    background: #97be2e none repeat scroll 0 0;
    border-color: #97be2e;
    color: #ffffff !important;
    transition: all 0.3s ease 0s;
}
.sharediv > h3{
  font-size: 20px;
  font-weight: 500;
  line-height: 20px;
  color: rgb(65, 65, 65)
}
.btn-arang{
  background-color: #97be2e;
  color:white;
  line-height: 1;
  width: 150px;
  text-align: center;
  vertical-align: middle;
  margin-bottom: 13px;
  margin-top: 10px;
}
.review-star{
  margin-top: 10px;
}
.price{
  color: #97be2e;
    font-size: 26px;
    font-weight: 600 !important;
    margin: 0;
    margin-top: 10px;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
}
.pak{
  border: 1px solid #ededed;

}
.data{
  text-align: center;
}
.sbox{
  padding: 5px;
  margin-left: 4px;
}
.pak > h2 {
    border-bottom: 1px solid #ededed;
    color: #414141;
    font-size: 15px;
    line-height: 1.47;
    margin: 0;
    padding: 14px 10px 10px;
    text-align: center;
}
.fa-star {
    color: #ffd800;
    text-align: center;
    padding: 0 5px;
}
.customlist li:before {
    content: "\f00c";
    padding: 0 10px 0 0;
    color: #9ac034!important;
    font-family: FontAwesome;
}
.customlist li{
  list-style-type: none;
  color: grey !important;
  font-size: 15px;
  line-height: 26px;
  font-family: "Helvetica Neue",sans-serif;
  margin-bottom: 10px;
}
.customlist{
  padding-left: 4px;
}
.one{
  color: #18293b;
  font-family: 'Raleway', sans-serif;
  font-size:15px;
  font-weight:700;
  padding-left: 5px;
  font-size: 15px;
    line-height: 27px;
    margin-bottom: 20px;
}
.second-paragraph{
  font-size: 15px;
  color:grey;
  padding: 10px;
}
@media (min-width: 768px){
  .col-md-7 {
    max-width: 54.333333%;
}
}
.first-paragraph{
  font-size: 18px;
  color:grey;
  padding: 10px;
  margin-bottom: 0px;
}
.second{
  font-weight: bold;
  font-family: 'Raleway', sans-serif;
  border-top:1px solid rgb(211, 210, 210);
  border-bottom:1px solid rgb(211, 210, 210);
  margin:0px;
  padding: 20px 0px 20px 5px;
  font-size:18px;
}
.cardslider{
  width:100%;
  margin-left: 14px;
}

.slide-image {
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    opacity: 0;
    transition: all .7s ease-in-out;
}

.slide-image img {
    width: auto;
    min-width: 100%;
    height: 100%;
}

.slide-image:hover + .carousel-controls label{
    opacity: 0.5;
}

.slide-container {
    display: block;
}


input:checked + .slide-container .slide-image {
    opacity: 1;
    transform: scale(1);
    transition: opacity 1s ease-in-out;
}

input:checked + .slide-container .carousel-controls label {
     display: block;
}

input:checked + .slide-container .nav label { display: block; }


.overlay {
    background-color: #080d15;
    height: 100%;
    opacity: .3;
    width: 100%;
    z-index: 2;
}
.overlay {
    position: absolute;
}

.slide-image {
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    opacity: 0;
    transition: all .7s ease-in-out;
}

.slide-image img {
    width: auto;
    min-width: 100%;
    height: 100%;
}



input:checked + .slide-container .slide-image {
    opacity: 1;
    transform: scale(1);
    transition: opacity 1s ease-in-out;
}

.item-1,
.item-2,
.item-3 {
	position: absolute;
  display: block;
	top: 7em;
  /* width: 60%; */
  text-align: center;
  font-size: 2em;
color:#fff;
	animation-duration: 20s;
	animation-timing-function: ease-in-out;
	animation-iteration-count: infinite;
}

.carousel-controls {
    position: absolute;
    top: -135px;
    left: 0;
    right: 0;
    z-index: 999;
    font-size: 80px;
    line-height: 600px;
    color: #fff;
}

.carousel-controls label {
    display: none;
    position: absolute;
    padding: 0 20px;
    opacity: 0;
    transition: opacity .2s;
    cursor: pointer;
}

.slide-image:hover + .carousel-controls label{
    opacity: 0.5;
}

.slides label:hover {
    opacity: 1;
}

.carousel-controls .prev-slide {
    width: 49%;
    text-align: left;
    left: 0;
}

.carousel-controls .next-slide {
    width: 49%;
    text-align: right;
    right: 0;
}

input:checked + .slide-container .carousel-controls label {
     display: block;
}



ul.slides {
    /* float: left;
    margin: 15px auto;
    padding: 0;
    width: 100%; */
   display: block;
    position: relative;
    height: 350px;
    margin: 0;
    padding: 0;
    overflow: hidden;
    list-style: none;
}

.slides * {
    user-select: none;
    -ms-user-select: none;
    -moz-user-select: none;
    -khtml-user-select: none;
    -webkit-user-select: none;
    -webkit-touch-callout: none;
}

ul.slides input {
    display: none;
}

.slides label:hover {
    opacity: 1;
}
.slider {
    float: left;
    margin: 15px auto;
    padding: 0 9px;
    width: 100%;
}
.cover{
  border-radius: 0px;
  border: 2px dashed rgb(151, 151, 151);
  width: 130px;
  height: 130px;
  padding-top: 50px;
  
}
.fullwidth_2{
  float: left;
  width: 60%;
  margin-left: 12px;
}
#file-input{ 
display: none;
}
.input-fake{
  float: left;
  display: inline-block;
  color: #97be2e;
  width: 183px;
  height: 163px;
  background-color: white;
  text-align: center;
  border: 1px solid #97be2e;
  font-weight: bold;
  padding:50px 30px;
  font-size: 14px;
  box-sizing: border-box;
}
.input-fake:hover{
  display: inline-block;
  background-color: #c0bdbd;
  color: Black;
  border: 3px dashed white;
  font-size: 14px;
}




.custext{
  font-size: 21px;
}
.fullwidth{
  width: 93% !important;
}

.col-md-3{
  max-width: 25% !important;
}
@media (max-width: 1100px) { 
    .col-md-3{
        min-width: 100%;
    }
    .fullwidth{
        min-width: 100% !important;
        }
.fullwidth_2{
  float: left;
  min-width: 100%;
}

.fullwidth{
  width: 100% !important;
}
.col-md-7{
        min-width: 100%;
        margin-top: 40px;
    }
 }
.col-md-3:last-child{
  position: absolute;
  right: 0px;
  max-width: 21% !important;
}

.scrollbar {
	margin-left: 0px;
	float: left;
	height:515px;
	width: 100%;
	background: #F5F5F5;
	overflow: auto;
  position: relative;
  overflow-x: hidden;
  
}

.style-3::-webkit-scrollbar-track {
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	background-color: #F5F5F5;
  margin-top: 15px;
}

.style-3::-webkit-scrollbar {
	width: 6px;
	background-color: #F5F5F5;
}

.style-3::-webkit-scrollbar-thumb {
	background-color: #000000;
}

.style-3::-webkit-scrollbar-thumb {
  background-color: #000000;
  border-radius: 10px;
}
.ad{
    padding-right: 0px !important;
    height: 77vh;
}



.overflow-hidden{
    overflow: hidden;
    width: 100%;
}
</style>
