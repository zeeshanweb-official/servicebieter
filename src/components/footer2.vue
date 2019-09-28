<template>
    <div class="fixed-bottom">
  <div class="row">
    <div class="sidefooter leftside"><div class="text-center">
      © 2017 Realtor. All Rights Reserved.
      </div></div>
    <div class="sidefooter rightside">
      <div class="row" style="margin:0px;">
       <div class="col-md-6 col-sm-7 text-right text-sm-left">
                    <a class="textmodrate" href="js:">Privacy Policy</a>
                </div>
                <div class="col-md-6 col-sm-3 text-right ">
                    <a class="textmodrate" href="js:">Terms of Use</a>
                </div>
      </div></div>
  </div>
    <!-- <div class="footer col-md-3">
        <div class="row pt-3">
        <div class="col-md-6 col-sm-6 col-xs-4 px-2 text-left">
              <div class="sec-bottom">&copy; 2017 Realtor. All Rights Reserved.</div>
            </div>
            <div class="col-md-6  col-sm-6 text-left px-0 row">
                <div class="col-md-1 col-sm-1 text-right px-0">
                </div>
               
            </div>
            </div>
        </div> -->
    </div>
 


</template>


<style>
 .textmodrate{
      color:#8297a8 !important;
      transition: color 0.3s ease;
      font-size: 13px;
      font-weight: 500;
    }
    .textmodrate:hover{
      color:#42ebff !important;
      text-decoration: none;
    }
.sidefooter{
  background-color: #f0f0f3;
  box-shadow: 0px -1px 0px 1px #dfdfe2;
  width: 270px;
  height: 40px;
  border-radius: 5px 5px 0px 0px;
  color: #8297a8;
  padding-top: 7px;
}
.leftside{
  position: fixed;
  left: 0px;
  bottom: 0px;
  font-size: 13px;
  font-weight: 500;
}
.rightside{
  position: fixed;
  right: 0px;
  bottom: 0px;
}
</style>