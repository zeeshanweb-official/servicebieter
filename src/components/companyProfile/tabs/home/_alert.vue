<template>
        <div class="alert klass">
               <div class="row">
                   <div class="col-md-9">
                       <strong>2015 Innovation Conference</strong>
                    <p>Interesting speakers, delicious food, do not miss this event!</p>
                   </div>
                   <div class="col-md-3">
                       <button class=" btn secondary" id="signup" href="js:">Sign up Today!</button>
                <div class="close3"><i class="fa fa-times-circle"></i></div>
                   </div>
               </div>
              
            </div>
</template>
<style>
      .alert{
        padding-left: 33px;
        padding-top: 15px;
        font-family: Arial, Helvetica, sans-serif;
    }
    .klass{
    color: white;
}
#signup{
    background-color: rgb(61, 139, 64);
    width: 175px;
    margin-top: 15px;
    color: white;
    font-size: 16px;
    font-weight: 600;
}
.close3{
    display: inline-block;
    position: absolute;
    right: 10px;
    top: -10px;
}
.fa-times-circle{
    font-size: 20px;
    color: #7bc57c;
    cursor: pointer;
}
.close3 :hover{
    color: rgb(61, 139, 64);
}
    .coverpage{
        background-color: #4caf50;
        margin: 25px 30px;
    border-radius: 4px;
    }
</style>