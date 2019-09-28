<template>
    <div>
        <div class="coverpage">
           <Alert></Alert>
        </div>
            <div class="row" style="width:100%; margin-left:0px; margin-top:50px;">
                <div class="col-md-12">
               <Paragraph></Paragraph>
                </div>
            </div>
        <AppSlider></AppSlider>
        <AppCards></AppCards>
         <div class="card card4" style="min-height: 400px;">
 
                    <div class="card-header newheader2 row p-0">
                        <div class="col-md-8 pl-0 profile-header">Recent Activity</div>
                        <div class="col-md-4 link pl-0">All Activity </div>
                             <Bgcard v-for="item in bgCardData" :key="item.index" :item="item"></Bgcard>
                    </div>
</div>
       
    </div>
</template>
<script>
import slider from './_slider'
import cards from './_cards'
import Bgcard from './_bgcard'
import Alert from './_alert'
import Paragraph from './_paragraph'
export default {
    components:{
        AppSlider:slider,
        AppCards:cards,
        Bgcard,
        Alert,
        Paragraph
    },
    data() {
        return {  
           
            bgCardData:[
                {
                    iconset:{warning:true,one:'fa-stack fa-lg', two:'fa fa-circle fa-stack-2x', three:'fa fa-usd fa-stack-1x'},
                    texts:"You registered for an event, Greater Atlanta Champer of Commerce 2015",
                    date:"2 Days Ago"
                },
                {
                    iconset:"fa fa-calendar-o fa-2x",
                    texts:"You made a payment in the amount of $34.99 to your membership account",
                    date:"4 Days Ago"
                },
                {
                    iconset:{one:'fa-stack fa-lg', two:'fa fa-circle fa-stack-2x', three:'fa fa-usd fa-stack-1x'},
                    texts:"You received a message from Bill Jones",
                    date:"5 Days Ago"
                },
                {
                    iconset:"fa fa-envelope fa-2x",
                    texts:"You registered for an event, at new fsd area",
                    date:"7 Days Ago"
                },
                {
                    iconset:"fa fa-eercast fa-2x",
                    texts:"this is nothing",
                    date:"15 Days Ago"
                },
            ]
        }
    },
}
</script>
<style>

.row-item{
    box-sizing: border-box;
    width: 99%;
    margin: 0%;
    padding: 10px;
    font-size: 14px;
    color: gray;
    font-weight: 400;
}
 .panel {
            background: #fff;
            border-top: 5px solid lightgray;

        }

        .panel .header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-size: 14px;
            font-weight: bold;
            padding: 10px;
            border-bottom: 1px solid lightgray;
            background: #fff;
            color: #000;
        }


.col-md-9 > strong{
    font-size: 18px;
}
.col-md-9> p{
    font-size: 14px;
}


  
</style>