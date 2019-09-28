<template>
           <div class="activitycontainer" style="width:100%">
                            <div class="row d-flex" style="justify-content:start;">
                                <div class="iconsec">
                                <span :class="item.iconset.one" v-if="typeof(this.item.iconset)==='object'" >
                                <i class="fa fa-warning fa-stack-3x" v-if="item.iconset.warning==true"></i>
                                        <i :class="item.iconset.two"></i>
                                        <i :class="item.iconset.three"></i>
                                <i class="fa fa-usd fa-stack-1x fa-inverse"></i>
                                </span>
                                <i v-else :class="item.iconset" style="margin-left:6px;color:rgb(138, 133, 133);"></i>
                                </div>
                                <div class="textsec">
                                    <div class="textspace">
                                <span>{{item.texts}}</span> 
                                <span class="btn btn-success btn-up btn-sm">View</span>
                            </div>
                            </div>
                            <div class="timesec">
                                 <div class="timespace">
                                {{item.date}}
                            </div>
                            </div>
                            </div>
                            <div class="px-2">
                                    <hr class="my-0"> 
                                </div> 

                        </div>
</template>
<script>
// Here you can add the code for different plugins
export default {
    
    props:['item'],
    // created(){
    //     console.log(this.item)
    // }
}
</script>
<style>
.fa-warning{
    position: absolute;
    top: -5;
    right: -8px;
    color: #ff9800;
    z-index: 13;
}
.iconsec{
    margin: 10px 10px 0px 20px;

}
.textsec{
    margin: 10px;
    margin-bottom: 0%;
}
.timespace{
    margin-top: 25px;
}
.btn-up{
 margin:10px;
 }
 .card-header  div:nth-last-child(5)  {
     margin-top: 10px;

}
 .card-header:nth-child(2){
     background-color: red;
 }
.activitycontainer{
    display: block;
}
       .card4{
        overflow: hidden;
        z-index: 130;
        border: none;
        border-top: 5px solid lightgray;
        margin: 0px;
        margin-left: 20px;
        margin-top: 20px;
        font-size: 14px;
        color:rgb(128, 128, 128)

    }
</style>