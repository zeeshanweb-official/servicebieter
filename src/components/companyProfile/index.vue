<template>
    <div>
        <div class="container-fluid px-0 mx-0 imagebg">
            <img class="profilepic" src="../../assets/images/profile-bannner.jpg" alt="profilebanner">
       <div class="row">
                <div class="col-md-3 col-sm-12 mt-1 newcls">
                    <div class="row mt-4">
                        <div class="col px-0">
                            
                        <AppProfile></AppProfile>    
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="row styel mx-0">
            <div class="col-md-12 px-0">
                <div class="coverdiv1">
                    <appTabs></appTabs>
                </div>
            </div>
        </div>
        
        
    </div>
</template>
<script>
import profile from './profile';
import tabs from './tabs';
export default {
    components:{
        AppProfile:profile,
        appTabs:tabs,
    }
}
</script>
<style>
.profilepic{
    height: 200px;
}
.imagebg{
    width: 98%;
    height: 200px;
}
.newcls{
    height: 100px;
    margin-left: 76px;
}
   .imagebg > img{
       height: 200px;
       width: 102%;
   }
   .styel{
       width: 100%;
   }
</style>