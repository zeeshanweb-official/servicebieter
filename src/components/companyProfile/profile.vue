<template>
    <div>
    <div class="container">
            <div class="card crdup card3">
                <div class="card-header newheader row p-0">
                    <div class="col-md-8 pl-0 profile-header">Profile ID:7262</div>
                    <div class="col-md-4 link pl-0">Edit Profile</div>
                </div>
                <div class="card-body p-0">
                    <div class="image">
                        <img src="../../assets/images/ideal_world.png" style="heigt:200px; width:298px; padding:15px;" alt="">
                    </div>
                    <div class="user">
                        <div class="first-p">Welcome, User
                            <strong>[Primary Organization Name]</strong>
                            <div class="details mt-2">
                                <i class="fa fa-map-marker"></i> <strong>Primary Chapter: </strong><span>Chicago IL</span>
                            </div>
                        </div>
                        <div class="btn-cover mb-2">
                            <div class="btn py-0 btn-block btn-alt">
                                <div class="row">
                                <div class="col-md-1"><div class="fa fa-check"></div></div>  
                                <div class="col-md-1"></div>   
                                <div class="col-md-9"><strong>Location: <p>Joined:27/08/2019</p></strong></div>    
                                </div>
                            </div>
                        </div>
                    </div>
                </div> 
            </div>
            <div class="card card3">
                <div class="card-header newheader row p-0">
                    <div class="col-md-8 pl-0 profile-header">Proffessional</div>
                    <div class="col-md-4 link pl-0"></div>
                </div>
                <div class="card-body p-0">
                    <div class="image text-center">
                        <img src="../../assets/images/SmartStaff-Logo-Rohan-02_1.png" style="heigt:200px; width:230px; padding:20px;" alt="">
                    </div>
                   <center>
                       <p class="smartstaff">What is SmartStaff</p>
                   </center>
                </div> 
            </div>
            <div class="card card3">
                <div class="card-header newheader row p-0">
                    <div class="col-md-8 pl-0 profile-header">Secure</div>
                    <div class="col-md-4 link pl-0"></div>
                </div>
                <div class="card-body p-0">
                    <div class="image text-center">
                    <i aria-hidden="true" class="fa fa-shield" style="font-size: 85px;color: rgb(151, 190, 46);margin-top: 15px;margin-left: 0px;"></i>
                    <p style="text-align: center;color: gray">100% Secure</p>
                    <p style="text-align: center;color: gray">Job is Done or Money back</p>
                    </div>
                </div> 
            </div>
            
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
.crdup{
    margin-top: -188px !important;
}
.smartstaff{
    font-size: 20px;
    font-weight: 500;
    font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
    margin-bottom: 30px;
}
.card-body{
    border: none !important;
    border-top: 1px solid rgb(253, 251, 251);
}
.btn-cover > .btn >.row>.col-md-9{
    text-align: start;
    height: 50px;
}
.fa-check{
    font-size: 30px;
    margin-top: 10px;
}
.btn-cover > .btn{
    margin-left: 0px;
    font-family: Arial, Helvetica, sans-serif;
    background-color: #4caf50;
    color: white;
}
.btn-cover > .btn > .col-md-1{
    padding-left: 0%;
}
.btn-cover{
    padding: 10px 20px;
}
.details{
    
    color: rgb(71, 71, 71);
}
.details>strong{
    font-size: 14px;
    font-weight: 700;
}
.details > span{
    display: block;
    margin-left: 40px;
    font-size: 14px;
    font-weight: 500;
}
.details > .fa-map-marker{
    font-size: 22px;
    padding: 0px 14px
}
.first-p{
    font-size: 22px;
    font-weight: 300;
    line-height: 24px;
    font-family: 'Raleway', Arial, Helvetica, sans-serif;
    padding: 10px 20px;

}
.first-p>strong{
    display: block;
    color: rgb(71, 71, 71);
    font-size: 14px;
    font-weight: 700;
    margin-top: 10px;

}
    .profile-header{
        color: gray;
        font-size: 14px;
        font-family: Arial, Helvetica, sans-serif;
        font-weight: 700;
    }
    .link{
    font-size: 14px;
    color: #03a9f4;
    font-weight: 400;
    text-align: end;
    }
    .card3{
        width: 300px !important;
        overflow: hidden;
        z-index: 130;
        border: none;
        border-top: 5px solid lightgray;
        margin: 20px 0px;
    }
    .newheader{
        width: 300px;
        margin-left: 0px;
        background-color: white;
        padding-left: 10px !important;
        height: 41px;
        padding-top: 10px !important;
    }
   
</style>