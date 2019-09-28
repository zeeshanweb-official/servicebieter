<template>
 <div class="wrapper">
     <div class="card shani">
    <h2 class="card-title text-center">{{ad.title}} <span class="newtext">{{ad.span}}</span></h2>
  <img class="card-img-top" src="@/assets/images/ideal_world.png" alt="Card image">
  <div class="card-body">
      <center>
          <div >
             
            </div>
             <router-link
              style="background-color:#97be2e; color:white; width: 140px; font-weight: 500; font-size:18px;"
              tag="a" class=" btn " to="/companyProfile">
                     Our Profile
                </router-link>
    </center>
        </div>
  <div class="container">
      <div v-for="ad in progress" :key="ad.index" class="innerdiv">
          <div class="row">
              <div class="col-md-12 col-sm-12 row">
                  <div class="col-md-2">
                      <h4 :class="ad.class" style="margin: 15px 0px 5px 18px; color:#777;"></h4>
                  </div>
                  <div class="col-md-10" style="font-size:14px; font-weight:600;">
                     {{ad.title}}
               <div class="progress">
                    <div class="progress-bar progress-bar-striped progress-bar-animated"  :style="{ width: ad.percent+'%' }"></div>
                </div>
                  </div>

              </div>
              
          </div>
      </div>
      
  </div>
</div>
</div>
</template>
<script>
export default {
      data() {
          return {
              ad:{
                  title:'Company Name',
                  span:'GMBH',
                  text_muted:'new'
              },
              progress:[
                  {
                      title:'95 % Jobs Done',
                      class:'fa fa-houzz',
                      percent:95,
                  },
                  {
                      title:'0 Hourly Jobs',
                      class:'fa fa-clock-o',
                      percent:2,
                  },
                   {
                      title:'5 Current Contracts',
                      class:'fa fa-file-text-o',
                      percent:75,
                  },
                  {
                      title:'30 Jobs Completed',
                      class:'fa fa-hourglass',
                      percent:70,
                  },
                 {
                      title:'150 Followers',
                      class:'fa fa-eye',
                      percent:30,
                  },
                 
                  {
                      title:'2500 $ earned',
                      class:'fa fa-money',
                      percent:99,
                  },
                  {
                      title:'10 Services for Sale',
                      class:'fa fa-credit-card',
                      percent:95,
                  },
                  {
                      title:'Jobs in Progress',
                      class:'fa fa-spinner',
                      percent:5,
                  },
              ]
          }
      },
    
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css?family=Raleway&display=swap');
.progress-bar{
    background-color: #97be2e;
   
}
.progress{
 height: 7px;
 border-radius: 0px;
}
.innerdiv{
    border-top:2px solid rgb(216, 215, 215);
    height: 50px;
}




.newtext{
    font-size: 7px;
    vertical-align: top;
    font-weight: 700;
}
.fa-shield{
    color:#97be2e ;
    font-size: 90px;
    margin-left: 90px;
}
.text16px{
    font-size: 16px !important;
}




.text-muted{
    color:#777;
    font-size: 21px;
    font-family: 'Raleway', sans-serif;
}
.card-title{
    font-family: 'Raleway', sans-serif;
    font-size: 30px;
    font-weight: 700;
    margin-top: 12px;
    padding-bottom: 20px;
    color: rgb(60, 60, 60);
    border-bottom: 1px solid rgb(224, 224, 224);
    
}
.card-img-top{
    height: 150px;
    width: 240px;
    margin-left: 30px;
    margin-top: 10px;
}
.card{
    width: 100%;
    border-top: 3px solid #3c8dbc;
}
</style>
