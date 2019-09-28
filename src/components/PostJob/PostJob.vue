<template>
<div>
<div class="scrollbar" id="style-3">
  <div class="bb-wizard container-fluid px-0 pb-2 m-0">
    <div style="margin-top: -4px;">
  <ul id="bb-wizard-steps" class="bb-wizard-steps markers bb-justified nav nav-tabs" role="tablist">
    <li class="nav-item">
      <a class="nav-link active" data-toggle="tab" href="#home" role="tab">
          <h4>
          <i class="fa fa-file-o"></i>
          Job Description
          </h4>
      </a>
    </li>
    <li class="nav-item">
      <a class="nav-link" data-toggle="tab" href="#profile" role="tab">
          <h4>
          <i class="fa fa-info"></i>
          Payment & work Plan
          </h4>
      </a>
    </li>
    <li class="nav-item">
      <a class="nav-link" data-toggle="tab" href="#messages" role="tab">
           <h4>
          <i class="fa fa-address-card"></i>
          View & Post
          </h4>
      </a>
    </li>
  </ul>

  <!-- Tab panes -->
</div>

</div>
<div class="row overflow-hidden mx-0">
      <div class="col-md-3  pr-0 ad">
        
          <appAd v-for="ad in ads" :key="ad.index" :ad="ad"></appAd>
      </div>
      <div class="col-md-7 px-1">
        <div class="scrollbar" id="style-3">
        <div class="tab-content container px-2">
    <div class="tab-pane px-0 active py-1" id="home" role="tabpanel">
      
<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Select the Service

</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Select Category  <span style="color:red;">*</span></label>
    <select class="form-control grn">
        <option v-for="i in 5" :key="i.index">Category {{i}}</option>    
     </select>
                    </div>
    <div class="col">
      <label for="first_name">Select Sub Category  <span style="color:red;">*</span></label>
   <select class="form-control grn">
      <option v-for="i in 5" :key="i.index">SubCategory {{i}}</option>
 </select>
                       </div>
  </div>
</form>
        </div> 

</div>
<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Select the Service Area
</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Work Area <span style="color:red;">*</span></label>
   <select class="form-control grn">
        <option v-for="i in 5" :key="i.index">Country{{i}}</option>     
    </select>
       </div>
    <div class="col">
      <label for="first_name">Select Bundesland <span style="color:red;">*</span></label>
      <select class="form-control grn">
        <option v-for="i in 5" :key="i.index">District{{i}}</option>
        </select>
    </div>
    <div class="col">
      <label for="first_name">City <span style="color:red;">*</span></label>
    <select class="form-control grn">
        <option v-for="i in 5" :key="i.index">City{{i}}</option>
      </select>
     </div>
  </div>
</form>
        </div> 

</div>
<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Describe your Project</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Project Title <span style="color:red;">*</span></label>
      <input type="text" id="first_name" class="form-control" placeholder="Project TItle">
    </div>
  </div>
  <div class="row">
    <div class="col">
      <textarea name="newtextarea" id="newtextarea" cols="98" rows="10"></textarea>
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Dokumente Hochladen</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col-md-3 p-0">
      <div class="btn cover"  data-toggle="modal" data-target="#myModal">
        <div class="btn-new">
        <i class="fa fa-plus" style="font-size:25px; color:#b9b4b4;"></i>
        </div>
      </div>
    </div>
    <div class="col-md-6"></div>
  </div>
</form>
        </div> 

</div>

    </div>
    <div class="tab-pane px-0 py-1" id="profile" role="tabpanel">
<div class="card fullwidth mb-3">
        <tabs3></tabs3>
</div>


<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Contract type</div>
        <div class="card-body">
          <tabs2>
            <template #tabs>
              <ul class="nav nav-tabs" role="tablist" style="margin-left: 190px; width: 65%;">
                  <li class="ml-2">&nbsp;</li>
                  <li class="nav-item">
                    <a class="nav-link" data-toggle="tab" href="#sc" role="tab">
                    <i class="fa fa-clock-o"></i> Standerd Contract
                    </a>
                  </li>
                  <li class="nav-item">
                  <a class="nav-link" data-toggle="tab" href="#exp" role="tab">
                 <i class="fa fa-fighter-jet"></i> Express Contract
               </a>
                  </li>
                </ul>
              
            </template>

            <template #details1>
            <div class="tab-pane p-2" id="sc" role="tabpanel">
            </div>
          </template>
            
            <template #details2>
            <div class="tab-pane p-2" id="exp" role="tabpanel">
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Recusandae, nemo. Quidem amet, molestiae labore beatae necessitatibus veniam incidunt, asperiores sapiente nihil perferendis expedita deleniti ducimus sequi tempora. Totam maiores vero inventore veniam, delectus iusto laboriosam quibusdam perferendis at architecto omnis ipsa eaque porro! Quaerat error, voluptas provident mollitia pariatur nulla..</p>
            </div>
          </template>
          </tabs2>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Select Work Start</div>
        <div class="card-body">
          <tabs2>
            <template #tabs>
              <ul class="nav nav-tabs" role="tablist" style="margin-left: 262px; width: 65%;">
                  <li class="ml-2">&nbsp;</li>
                  <li class="nav-item">
                    <a class="nav-link" data-toggle="tab" href="#bd" role="tab">
                    <i class="fa fa-clock-o"></i> By Date
                    </a>
                  </li>
                  <li class="nav-item">
                  <a class="nav-link" data-toggle="tab" href="#agree" role="tab">
                 <i class="fas fa-hands-usd"></i> Agreement
               </a>
                  </li>
                </ul>
              
            </template>

            <template #details1>
            <div class="tab-pane p-2" id="bd" role="tabpanel">
              <input class="form-control" style="margin:10px 0px 10px 270px; width:152px; display:inline" type="date" name="datetime" id="datetime">
              <span class="calicon" style="padding:3px 4px 5px 4px; background-color:lightgray;">
              <i class="fa fa-calendar-o"></i>
              </span>
            </div>
          </template>
            
            <template #details2>
            <div class="tab-pane p-2" id="agree" role="tabpanel">
              
             </div>
          </template>
          </tabs2>
        </div> 

</div>
<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Select Work Delivery</div>
        <div class="card-body">
          <tabs2>
            <template #tabs>
              <ul class="nav nav-tabs" role="tablist" style="margin-left: 262px; width: 65%;">
                  <li class="ml-2">&nbsp;</li>
                  <li class="nav-item">
                    <a class="nav-link" data-toggle="tab" href="#byd" role="tab">
                    <i class="fa fa-clock-o"></i> By Date
                    </a>
                  </li>
                  <li class="nav-item">
                  <a class="nav-link" data-toggle="tab" href="#agreed" role="tab">
                 <i class="fas fa-hands-usd"></i> Agreement
               </a>
                  </li>
                </ul>
              
            </template>

            <template #details1>
            <div class="tab-pane p-2" id="byd" role="tabpanel">
              <input class="form-control" style="margin:10px 0px 10px 270px; width:152px; display:inline" type="date" name="datetime" id="datetime">
              <span class="calicon" style="padding:3px 4px 5px 4px; background-color:lightgray;">
              <i class="fa fa-calendar-o"></i>
              </span>
            </div>
          </template>
            
            <template #details2>
            <div class="tab-pane p-2" id="agreed" role="tabpanel">
              
             </div>
          </template>
          </tabs2>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Select Company Skills</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col"> 
      <SearchBox></SearchBox>
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Select Company characteristic</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col"> 
      <SearchBox></SearchBox>
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Dokumente Hochladen</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col-md-3 p-0">
      <div class="btn cover"  data-toggle="modal" data-target="#myModal">
        <div class="btn-new">
        <i class="fa fa-plus" style="font-size:25px; color:#b9b4b4;"></i>
        </div>
      </div>
    </div>
    <div class="col-md-6"></div>
  </div>
</form>
        </div> 

</div>



    </div>
    <div class="tab-pane px-0 py-1" id="messages" role="tabpanel">

      <div class="card fullwidth mb-3">
        <div class="card-header custext p-1">
          <div class="row">
            <div class="col-md-8"> Contract Type</div>
            <div class="col-md-3 text-right" style="font-size:16px;">
              <small>Job ID:7262</small>
            </div>
          </div>
        </div>
        <div class="card-body">
          <form id="myForm">
  <div class="row mb-5">
    <div class="col">
      <div class="ques">Inquire Type:</div>
      <div class="answe">Agreement</div>
    </div>
    <div class="col text-right">
      <div class="ques">Contract Type:</div>
      <div class="answe">Express</div>
      </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Describe your Project</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Project Title <span style="color:red;">*</span></label>
      <input type="text" id="first_name" class="form-control" placeholder="Project TItle">
    </div>
  </div>
  <div class="row">
    <div class="col">
      <textarea name="newtextarea" id="newtextarea" cols="98" rows="10"></textarea>
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Project Tasks
</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <div>
                      <div class="notice notice-success btn">
                        <strong>Change</strong> Background
                        <div style="float: right;margin-right:100px; ">
                        </div>
                      </div>
                    </div>
    </div>
    <div class="col">
      <div>
                      <div class="notice notice-success btn">
                        <strong>Change</strong> Background
                        <div style="float: right;margin-right:100px; ">
                        </div>
                      </div>
                    </div>
    </div>
  </div>
  <div class="row">
    <div class="col">
      <div>
                      <div class="notice notice-success btn">
                        <strong>Change</strong> Background
                        <div style="float: right;margin-right:100px; ">
                        </div>
                      </div>
                    </div>
    </div>
    <div class="col">
      <div>
                      <div class="notice notice-success btn">
                        <strong>Change</strong> Background
                        <div style="float: right;margin-right:100px; ">
                        </div>
                      </div>
                    </div>
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Work Start / Work Delivery
</div>
        <div class="card-body">
          <form id="myForm">
          <div class="row mb-5">
              <div class="col">
                <div class="ques">Work Start :</div>
                <div class="answe">Agreement</div>
              </div>
              <div class="col text-right">
                <div class="ques">Work Delivery :</div>
                <div class="answe">27/08/1996</div>
                </div>
            </div>
</form>
        </div> 

</div>
<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Project Files</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <span style="font-size:14px; color: gray;">Work Desc...</span>
    </div>
    <div class="col">
      <span style="font-size:14px; color: gray;">Work Desc...</span>
    </div>
    <div class="col">
      <span style="font-size:14px; color: gray;">Work Desc...</span>
    </div>
    <div class="col">
      <span style="font-size:14px; color: gray;">Work Desc...</span>
    </div>
  </div>
</form>
        </div> 

</div>
<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Project Tasks</div>
        <div class="card-body">
          <form id="myForm">
  <div v-for="i in 2" :key="i.index" class="row">
     <div class="col" v-for="j in 4" :key="j.index">
      <div>
                      <div class="notice notice-success btn">
                        <strong>ON time</strong>
                        <div style="float: right;margin-right:100px; ">
                        </div>
                      </div>
                    </div>
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Budget And Payment
</div>
        <div class="card-body">
          <form id="myForm">
          <div class="row mb-2 ml-3">
              <div class="col">
                <div class="ques">Budget Type :</div>
                <div class="answe">Fix / Hourly</div>
              </div>
              <div class="col text-right mr-3">
                <div class="ques">Total Budget :</div>
                <div class="answe">2700$</div>
                </div>
            </div>
          <div class="row ml-3">
              <div class="col">
                <div class="ques">Budget is :</div>
                <div class="answe">Fix </div>
              </div>
              <div class="col text-right mr-3">
                <div class="ques">Payouts :</div>
                <div class="answe">After Finish</div>
                </div>
            </div>
          <div class="row mt-4">
              <div class="col">
                <input type="radio" name="fix" id="accept" class="form-contro"> Accept Policy And Terms
              </div>
            </div>
          <div class="row">
              <div class="col">
                  <input type="radio" name="fix" id="accept" class="form-contro"> Accept Privacy Terms
                </div>
            </div>
</form>
        </div> 

</div>


    </div>
    <!-- <div class="tab-pane px-0 py-1" id="settings" role="tabpanel">
      <div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Firma</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Your Company Name <span style="color:red;">*</span></label>
      <input type="text" id="first_name" class="form-control" placeholder="Company Name">
    </div>
    <div class="col">
      <label for="first_name">Company Type <span style="color:red;">*</span></label>
      <input type="text" class="form-control" placeholder="Company Type">
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Firma</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Your Company Name <span style="color:red;">*</span></label>
      <input type="text" id="first_name" class="form-control" placeholder="Company Name">
    </div>
    <div class="col">
      <label for="first_name">Company Type <span style="color:red;">*</span></label>
      <input type="text" class="form-control" placeholder="Company Type">
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Firma</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Your Company Name <span style="color:red;">*</span></label>
      <input type="text" id="first_name" class="form-control" placeholder="Company Name">
    </div>
    <div class="col">
      <label for="first_name">Company Type <span style="color:red;">*</span></label>
      <input type="text" class="form-control" placeholder="Company Type">
    </div>
  </div>
</form>
        </div> 

</div>

<div class="card fullwidth mb-3">
        <div class="card-header custext p-1">Firma</div>
        <div class="card-body">
          <form id="myForm">
  <div class="row">
    <div class="col">
      <label for="first_name">Your Company Name <span style="color:red;">*</span></label>
      <input type="text" id="first_name" class="form-control" placeholder="Company Name">
    </div>
    <div class="col">
      <label for="first_name">Company Type <span style="color:red;">*</span></label>
      <input type="text" class="form-control" placeholder="Company Type">
    </div>
  </div>
</form>
        </div> 

</div>


    </div> -->
  </div>
      </div>
      </div>
      <div class="col-md-3 pr-0 ad">
          <appAd v-for="ad in ads" :key="ad.index" :ad="ad"></appAd>
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
  <customFooter></customFooter>
</div>

</template>
<script>
import ad from '../BeMember/ad'
import $ from 'jquery';
import tabs3 from './tabs/tabs3'
import tabs2 from './tabs/tabs2'
import SearchBox from './tabs/tabSearchBox'
import customFooter from '../footer2'
window.$= $;
export default {
  mounted() {
      $("#hideitem").hide();
    },
    beforeRouteEnter (to, from, next)  {
      $("#hideitem").hide();
      next();
    },
    beforeRouteLeave (to, from, next) {
      $("#hideitem").show();
      next();
    },
    data() {
      return {
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
                ],
               
                }
    },
    components:{
        appAd:ad,
        customFooter,
        tabs3,
        tabs2,
        SearchBox,
        
    },
   
    
}
</script>



<style scoped>

.ques{
  background-color:#E7E6E6;
  display:inline-block;
  padding: 0px 5px;
}
.answe{
  background-color: #F2F2F2;
  display: inline-block;
  padding: 0px 5px;

}
.notice {
    padding: 15px;
    background-color: #fafafa;
    border-left: 6px solid #97be2e;
    color: #97be2e;
    margin-bottom: 10px;
    -webkit-box-shadow: 0 5px 8px -6px rgba(0, 0, 0, .2);
    -moz-box-shadow: 0 5px 8px -6px rgba(0, 0, 0, .2);
    box-shadow: 0 5px 8px -6px rgba(0, 0, 0, .2);
}
.notice:active, .notice.active {
    background-image: none;
    outline: 0;
    -webkit-box-shadow: inset 0 3px 5px rgba(0,0,0,0.125);
    box-shadow: inset 0 3px 5px rgba(0,0,0,0.125);
}
.btn:hover, .btn:focus {
    color: #333;
    text-decoration: none;
}



#newtextarea{
  margin-top: 10px;
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
  width: 73%;
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

.form-control{
  font-size: 14px;
  border-color: #97be2e !important;
  padding: 2px;
}
select.form-control{
  padding: 0px;
  max-height: 33px;
}


.custext{
  font-size: 21px;
}
.fullwidth{
  width: 100% !important;
}

.col-md-3{
  max-width: 21% !important;
}
.col-md-3:last-child{
  position: absolute;
  right: 0px;
}
.scrollbar {
	margin-left: 0px;
	float: left;
	height:515px;
	width: 100%;
	background: #F5F5F5;
	overflow-y: auto;
  position: relative;
  overflow-x: hidden;
}

#style-3::-webkit-scrollbar-track {
	-webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
	background-color: #F5F5F5;
}

#style-3::-webkit-scrollbar {
	width: 6px;
	background-color: #F5F5F5;
}

#style-3::-webkit-scrollbar-thumb {
	background-color: #000000;
}

#style-3::-webkit-scrollbar-thumb {
  background-color: #000000;
  border-radius: 10px;
}
.ad{
    padding-right: 0px !important;
    height: 77vh;
}
.nav0link.active{
  background-color: transparent !important;
  border-top: 2px solid #bd2522  !important;
  border-bottom: 2px solid #bd2522 !important;
  border-left: none !important;
  border-right: none !important;
  color: #9ac034  !important;
  border-radius: 0% !important;
}
.nav0link.active:hover{
  background-color: #eee !important;    
  border-top: 2px solid #bd2522 !important;
  border-bottom: 2px solid #bd2522 !important;
}


.overflow-hidden{
    overflow: hidden;
    width: 100%;
}
.bb-wizard{
    overflow: hidden;
}
.bb-wizard-steps>li{
    text-align: center;
}
.bb-wizard-steps>li>a{
    padding: 8px;
    background-color: #e6ecef;
}
.bb-wizard-steps>li>a>h4{
    font-size: 16px;
}
a.active {
    background-color: #97be2e !important;
    box-shadow: inset 0px -4px 0px 0px #97be2e;
    color: white !important;
}
    .bb-wizard-btnNext {
      color: black;
      cursor: pointer;
    }
    .bb-wizard-steps h4 .fa{
    padding-right: 5px;
}
.bb-wizard-steps h4{
    font-weight: 600;
    font-size: 1.6rem;
    margin: 0;
    padding: 7px 74px;
    line-height: 1.4rem;  
    /* text-shadow: 1px 1px 2px rgba(0, 0, 0, .3); */
  }
  
  .bb-wizard hr{
    border: 0; margin: .8rem 0 .8rem 0; padding: 0;
    border-top: .1rem solid rgba(60, 60, 60 , .1);
    border-bottom: .1rem solid rgba(255, 255, 255 , .5);
  }
 .bb-wizard, .bb-wizard-page{
      /* margin: 3rem; */
      /* padding: 1rem; */
      border-radius: .2rem;
      border: .1rem solid rgba(0, 0, 0, .05);
      box-shadow: none !important;
      /* box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.2); */
      border-width: .1rem 0 0 0;
      
  }
  
  .bb-wizard-page{margin: 0;
      border: 0;
      box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.2);
      /* overflow-y: scroll; */
  /*    height: calc(100vh / 1.6 + 4rem); */
  }
  
  .bb-wizard-steps{
    font-size: .85rem;
    display: inline-block;  
    position:relative;
    list-style: none;
    counter-reset: bb-wizard-counter;  
  }
  
  .bb-wizard-steps li{
    margin-bottom: .25rem;
    counter-increment: bb-wizard-counter;
  }
  
  .bb-wizard-steps.markers label{
      display: inline-block; position: relative;
      padding: 0 0 0 1.8rem;
      margin: 0;
      text-align: left;
      vertical-align: top;
  }
  
  .bb-wizard-steps.markers label:before{
      display: none !important;
    content: counter(bb-wizard-counter);
    display: inline;
    font-size: 4rem; font-weight: 600;
    line-height: 2rem;
    text-align: left;
    color: inherit;
    opacity: 0.1;
    position: absolute;
    left: -1rem; top: .1rem;
    z-index: 11; 
   }
  
  .bb-wizard-steps li {
      display: block;
      width: 24.99%;
      background: rgba(4,4,4,.1);
      position:relative;
      float: left;
      --box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.2);
       border-radius: .2rem;
       --border-top: .01rem solid rgba(230, 230, 230, 0.2);
       --border-left: .0rem solid rgba(0, 0, 0, 0.02);
       --border-right: .0rem solid rgba(0, 0, 0, 0.02);
       
  }
  
  .bb-wizard-steps li a{
    color: #555;
    padding-left: 2.4rem;
    padding-left: 1.6rem;
  }
  .bb-wizard-steps li:first-of-type a{
    padding-left: 1.6rem;
  }
  .bb-wizard-steps li:last-of-type a{
    padding-right: 1.6rem;
  }
  
  .bb-wizard-steps li:last-of-type a:before,
  .bb-wizard-steps li:last-of-type a:after{
    visibility: hidden;
    }
  
  
  .bb-wizard-steps a:before, .bb-wizard-steps a:after {
    z-index: 1;
      height: 50%;
      width: 1rem;
      right: 0%;    
      margin-right: -.5rem;
      padding: 0;
      display: block;
      content: '';
      background: inherit;
      position:absolute;
      transform: skewX(20deg);
       box-shadow: .2rem 0 0 0 rgba(0, 0, 0, 0.2);
     /*
      box-shadow: inset 2px 0px 5px 2px rgba(50, 50, 50, 0.75); 
      */
      border-radius: 80% .1rem 0 0;
      border: solid rgba(255, 255, 255, 0.9);
      border-width: 0 .3rem 0 0;
      
  }
  
  .bb-wizard-steps a:before{top: 0%;}
  
  .bb-wizard-steps a:after{
    transform: skewX(-20deg);
    border-radius: 0 0 .1rem 80%;
    border-width: 0 .3rem 0 0;
    bottom: 0%;
    box-shadow: .2rem 0 0 0 rgba(0, 0, 0, 0.3);
  
  }
  
  .bb-wizard-steps a>*{cursor: pointer;}
  .bb-wizard-steps a{
    cursor: pointer;
    display: block;
    position: relative;
    padding: 1rem 1.2rem 1rem 1.6rem;
    border-radius: .15rem .15rem .15rem .15rem;
    background: #FFF;  
    /*
    border: solid .0rem rgba(255,255,255,.2);
    border: solid .1rem rgba(0,0,0,.05);
    */
    
    border-left: solid .1rem rgba(100,100,100,.1);
    border-right: solid .1rem rgba(100,100,100,.1);
    border-top: solid .1rem rgba(0,0,0,.1);
    border-bottom: solid .1rem rgba(0,0,0,.12);
    box-shadow:
      0px 1px .2rem 1px rgba(0, 0, 0, 0.1),
      inset 0px 0px 0px 1px rgba(250, 250, 250, 0.1)
      ;
    
  }
  
  .bb-wizard-steps a{transition: background-color .3s ease, color .3s ease;}
  .bb-wizard-steps a:hover{background: #444; color: #fff;
    transition:
            background-color .3s ease,
            color .3s ease;
  }
  
  .bb-wizard-steps li.active a{background: #96c03d; color: #fff}
  .active-red{
      border-bottom: 3px solid red;
  }
  .bb-wizard-steps.bb-justified {
	 display: table;
	/* padding-left: 16px;
	 */
	 margin-bottom: -2px;
	 width: 100%;
}
 .bb-wizard-steps.bb-justified:before, .bb-wizard-steps.bb-justified:after {
	 display: table;
}
 .bb-wizard-steps.bb-justified li {
	 display: table-cell;
	 float: none;
}
</style>
