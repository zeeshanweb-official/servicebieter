<template>
    <div >
        <div class="">
  <ul class="nav nav-tabs bg-custom" role="tablist">
    <li class="ml-2">&nbsp;</li>
    <li class="nav-item">
      <a class="nav-link nav-link3 active" data-toggle="tab" href="#home" role="tab">Home</a>
    </li>
    <li class="nav-item">
      <a class="nav-link nav-link3" data-toggle="tab" href="#profile" role="tab">Jobs</a>
    </li>
    <li class="nav-item">
      <a class="nav-link nav-link3" data-toggle="tab" href="#messages" role="tab">Offers</a>
    </li>
    <li class="nav-item">
      <a class="nav-link nav-link3" data-toggle="tab" href="#settings" role="tab">Reviews</a>
    </li>
     <li class="nav-item">
      <a class="nav-link nav-link3" data-toggle="tab" href="#referneces" role="tab">Refrences</a>
    </li>
     <li class="nav-item">
      <a class="nav-link nav-link3" data-toggle="tab" @click="infoclicked" href="#info" role="tab">Info</a>
    </li>
  </ul>

  <!-- Tab panes --> 
  <div class="tab-content tab-content2">
    <div class="tab-pane p-2 active" id="home" role="tabpanel">
     <AppHome></AppHome>
    </div>
    <div class="tab-pane p-2" id="profile" role="tabpanel">
      <div class="container">
           <tableRows v-for="item in tablelist" :options="item" :key="item.index" ></tableRows>
      </div>
    </div>
    <div class="tab-pane p-2" id="messages" role="tabpanel">
      <div class="container-fluid">
        <div class="row" style="margin:10px;">
          <div v-for="service in services" :key="service.index" :service='service' class="col-md-4 px-0">
          <appService :service="service"></appService>
          </div>
        </div>
      </div>
    </div>
    <div class="tab-pane p-2" id="settings" role="tabpanel">
      <div class="row" style="margin-left:0px; margin-right:0px; width:970px;">
        <div class="bigdiv">
          <AppReview></AppReview>
        </div>
        <div class="smalldiv">
          <div class="ratingsdiv">
              <div class="row" style="width:100%;">
                <div class="col-md-12  pr-0 ml-2">
                  <div v-for="i in services" :key="i.index">
                    <i v-for="star in i.stars" :key="star.index" style="color:#fac917" class="fa fa-star mx-2"></i>
                      <div class="newfixedl">
                        <p  v-for="i in services" :key="i.index">{{i.stars}}.0/5.0</p>
                      </div>
                  </div> 
                </div>
              </div>
          </div>
          <div class="totalreview text-center">
            <h4 style="font-size">Total Review</h4>
            <p>4.0/5.0</p>
          </div>
          <div class="rewiews">
            <div class="form-group">
            <select class="form-control" id="sel1">
              <option>Sort By</option>
              <option>A to Z</option>
              <option>Z to A</option>
              <option>By Price</option>
            </select>
          </div>
          <div v-for="review in reviews" :key="review.index" class="rewiew">
            <div class="row">
              <div class="col-md-3">
                <div class="imground">
                  <img src="../../assets/images/avtar.jpg" alt="">
                </div>
              </div>
              <div class="col-md-9">
                    <strong style="font-size:12px;">Order ID : {{review.order}}</strong>
                    <p>{{review.date}}</p>
                    <strong style="font-size:12px;">{{review.price}}$</strong>
                    <br>
                    <i v-for="i in review.stars" :key="i.index" class="fa fa-star" style="color:#fac917"></i>
                
              </div>
            </div>
          </div>
          </div>
        </div>
      </div>
    </div>
    <div class="tab-pane p-2" id="referneces" role="tabpanel">
        <div class="col-sm-12 pt-4 pb-0">
              <div class="agent-property">
                <div class="row">
                    <MyService v-for="image in images" :key="image.index" :image="image.image"></MyService>
                  </div>
                </div>
              </div>
    </div>
    <div class="tab-pane p-2" id="info" role="tabpanel">
      <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d4867.228952306545!2d9.652084!3d52.413663!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47b073e0501e577d%3A0xbedcb3851d18d688!2sAlte%20St%C3%B6ckener%20Str.%2070%2C%2030419%20Hannover%2C%20Germany!5e0!3m2!1sen!2sin!4v1567380642016!5m2!1sen!2sin" width="950"  height="450" frameborder="0" style="border:0; margin-left:20px;" allowfullscreen=""></iframe>
      <div class="lastdiv">
        <lastdiv></lastdiv>
      </div>
    </div>
  </div>
</div>
    </div>
</template>
<script>
import AppHome from './tabs/home/index';
import AppReview from './tabs/review/index';
import tableRows from '../JobPortal/tableRows'
import service from '../Services/BuyServices/otherservice'
import simpleservice from '../Services/myservice'
import lastdiv from './tabs/review/new tabs'
export default {
  components:{
    AppHome,
    AppReview,
    tableRows,
    appService:service,
    MyService:simpleservice,
    lastdiv
  },
  data() {
    return {
       images:[
    {
      image:'01.jpg'
    },
    {
      image:'02.jpg'
    },
    {
      image:'03.jpg'
    }
    ],
      reviews:[
        {
          order:334499,
          date:'27 aug, 2019',
          price:23,
          stars:5
        },
        {
          order:333399,
          date:'27 aug, 2016',
          price:345,
          stars:3
        },
        {
          order:3345566,
          date:'27 aug, 2018',
          price:234,
          stars:2
        },
        {
          order:3341232,
          date:'27 aug, 2017',
          price:2245,
          stars:4
        },
        {
          order:4567854,
          date:'27 aug, 2015',
          price:675,
          stars:5
        },
        {
          order:334499,
          date:'27 aug, 2019',
          price:238,
          stars:2
        },
      ],
       services:[
          {
            classes:'',
            id:1,
            title:'Awesome Villa',
            address:'gulistan Colony SHahkot',
            image:'r-property-img.jpg',
            price:"$450",
            stars:4
          },
          {
            classes:'',
            id:2,
            title:'Good Thing',
            address:'gulistan Colony no 2 Faisalabad',
            image:'blog-full-4.jpg',
            price:"$400",
            stars:3
          },
          {
            classes:'',
            id:3,
            title:'Very Nice Home',
            address:'Housing Society Faisalabad',
            image:'blog-full-5.jpg',
            price:"$400",
            stars:3
          },
          { 
            classes:'',
            id:4,
            title:'Very Good House',
            address:'Mustafaabad Housing Society Faisalabad',
            image:'blog-full-4.jpg',
            price:"$405",
            stars:2
          },
          {
            classes:'',
            id:5,
            title:'Very Good House',
            address:'Mustafaabad Housing Society Faisalabad',
            image:'blog-full-3.jpg',
            price:"$405",
            stars:2
          },
          {
            classes:'',
            id:6,
            title:'Very Good House',
            address:'Mustafaabad Housing Society Faisalabad',
            image:'blog-full-5.jpg',
            price:"$405",
            stars:2
          },
          
      ],
       tablelist:[
                {
                    special:true,
                    link:'Change Coach / Organisationsentwickler (m/w/d)',
                    address:' Gulistan Colony',
                    map:'Shahkot Distt Nankana sahib',
                    details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda aliquam iusto voluptate nisi dolores at nemo quaerat veritatis ratione dignissimos.'
                },
                {
                    special:true,
                    link:'new Title Text',
                    address:'Mustafabad ',
                    map:'Faisalabad',
                    details:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda aliquam iusto voluptate nisi dolores at nemo quaerat veritatis ratione dignissimos.'
                },
                ],
    }
  },
 methods: {
    infoclicked(){
      setTimeout(() => {
        $(".newone")[0].click();
      }, 200);
    }
  },
    
}
</script>
<style>
#newone,#newtwo, #newThree{
  margin-left: 20px;
  border: 1px solid gray;
  width: 885px;
  margin-top: 10px;
  border-radius: 4px;
  margin-left: 38px;
}
.tabswesy{
  border: none !important;
  margin-left: 20px;
}
.tabswesy>li:nth-child(2){
  margin-left: 10px;
}
.newone{
  border: none !important;
  width:290px;
  border: 1px solid gray !important;
  margin:0px 2px 0px 2px;
  border-radius: 5px;
  height: 50px;
  text-align: center;
  font-size: 14px;
  font-weight: 600;
}
.lastdiv {
  background-color: white;
  width: 950px;
  min-height: 100px;
  margin: 40px 0px 10px 10px;
}
.imground>img{
  border-radius: 49%;
  width: 40px;
  height: 40px;
  margin-top: 100%;
  margin-left: 10px;
}
.rewiew{
  border: 1px solid lightgray;
  width: 100%;
  margin: 10px 0px; 
}
.totalreview  {
    background-color: #f3f3f3;
    text-align: center;
    padding: 10px;
}
.newfixedl>p{
  margin: 0px;
}
.newfixedl{
  position: absolute;
  right: 10px;
  top: 0%;
}
.ratingsdiv{
  width: 100%;
  height: 200px;
  background-color: white;
  margin-top: 27px;
  padding-top: 10px;
  border-top: 5px solid lightgray;
}
.cover-2{
  padding: 20px 20px 20px 30px;
  background-color: green;
}
.tab-content2{
    padding-left: 370px;
     background-color:#f6f6f6;
     min-height: 1000px;
}
.nav-link3 {
    background-color: transparent;
    font-size: 14px;
    font-weight: 500;    
    color: #eee;

}
.nav-link3.active{
 background-color: transparent !important;
    color: #eee !important;
    border-color: transparent !important; 
    border-bottom: 5px solid #eee !important;
}
.nav-link3:hover{
     border-color: transparent !important; 
     color: #eee;
}

.bg-custom{
    background-color: #4caf50;
    z-index: -3;
    padding-left: 410px;
    border: none !important;
    font-size: 20px;
}
</style>