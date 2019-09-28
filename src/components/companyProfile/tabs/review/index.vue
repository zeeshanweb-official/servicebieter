<template>
<div>
<div class="coverpage newpage">
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
</div>
          <div class="panel panel2" id="activity">
                    <div class="header" style="color:gray; font-size:14px; font-weight:700; line-height:20px;">About Us</div>
                    <div class="item row row-item">
                        <p>
                        What is Lorem Ipsum? Lorem Ipsum is simply dummy
                        text of the printing and typesetting industry.
                        Lorem Ipsum has been the industry's standard
                        dummy text ever since the 1500s, when an unknown
                        printer took a galley of type and scrambled it
                        to make a type specimen book. It has survived
                        not only five centuries, but also the leap into
                        electronic typesetting, remaining essentially
                        unchanged. It was popularised in the 1960s with
                        the release of Letraset sheets containing Lorem
                        Ipsum passages, and more recently with desktop
                        </p>

                    </div>
                </div>
                <div class="sliderapp">
                    <appSlider></appSlider>
                </div>
                <div class="mulcardsbody">
                <mulcards></mulcards>
               <div class="card card4" style="min-height: 400px;">
 
                    <div class="card-header newheader2 row p-0">
                        <div class="col-md-8 pl-0 profile-header">Recent Activity</div>
                        <div class="col-md-4 link pl-0">All Activity </div>
                             <singleCard v-for="item in bgCardData" :key="item.index" :item="item"></singleCard>
                    </div>
</div>
                </div>
</div>
</template>
<script>
import slider from '../home/_slider'
import cards from '../home/_cards'
import bigcard from '../home/_bgcard'
export default {
    components:{
        appSlider:slider,
        mulcards:cards,
        singleCard:bigcard
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
.mulcardsbody{
    margin-left: 0px;
    width: 755px;
}
.sliderapp{
    width:745px;
}
.panel2{
    margin-left: 15px;
    width: 730px;
}
.bigdiv{
    width: 720px;
    float: left;
}
.smalldiv{
    width: 220px;
    float: left;
    margin-left: 30px;
}
#signup{
    width: auto;
}
.newpage{
    width:700px !important;
    overflow:hidden;
    margin-left: 10px;
    margin-left: 30px;
}
.klass{
    margin-bottom:0px;
}
    
</style>