<template>
<div>

     <div  class="row mb-3" v-if="options.special===true" style="padding-bottom:12px; width:100% !important; margin-left:15px;">
                <div class="col-md-2" style="border-right:1px solid rgb(204, 198, 198);">
                    <img class="littleimage" src="../../assets/images/man.png" alt="">
                </div>
                <div class="col-md-10">
                    <h5 style="color:gray;">
                        <a class="good" href="js:">{{options.link}}</a>
                    </h5>
                    <div class="text-muted">
                    <i class="fa fa-building"></i>
                    {{options.address}} &nbsp;&nbsp;&nbsp;&nbsp;
                    <i class="fa fa-map-marker"></i>
                    {{options.map}}
                    </div>
                   {{options.details}} 
                </div>
            </div>
     <div v-else class="row mb-3" style="padding-bottom:12px;">
                <div class="col-md-2" style="border-right:1px solid rgb(204, 198, 198);">
                    <img class="littleimage" src="../../assets/images/man.png" alt="">
                </div>
                <div class="col-md-10">
                    <h5 style="color:gray;">
                        <a class="good" href="js:">{{options.link}}</a>
                    </h5>
                    <div class="text-muted">
                    <i class="fa fa-building"></i>
                    {{options.address}} &nbsp;&nbsp;&nbsp;&nbsp;
                    <i class="fa fa-map-marker"></i>
                    {{options.map}}
                    </div>
                   {{options.details}} 
                </div>
            </div>
    </div>
</template>
<script>
export default {
    props:['options'],
    // created() {
    //     console.log(this.options)
    // },
}
</script>
<style scoped>
.good{
    text-decoration: none !important;
}
.text-muted{
    font-size:14px;
}
    .littleimage{
        height: 90px;
        width: 90px;
        margin-left: 10px;
        margin-top: 6%;
    }
    .row{
        background-color: rgb(238, 238, 238);
        margin-left: 1px;
        border-left: 4px solid #97be2e;
        width: 1190px;
    }
    
</style>