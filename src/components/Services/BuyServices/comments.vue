<template>
    <div>
         <div class="feedback">
            <div class="coment">
                <appcomment v-for="comment in comments" :key="comment.index" :comment="comment"></appcomment>
            </div>
        </div>
    </div>
</template>
<script>
import comment from './comment'
export default {
    components:{
        appcomment:comment,
    },
    data() {
        return {
            comments:[
                {flag:'https://www.animatedimages.org/data/media/850/animated-pakistan-flag-image-0001.gif',name:'Zeeshan', country:'Pakistan', icon:'pk', star:3 , time: '2 months', date:'14 Aug 2019', words:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla, dolorum.'},
                {flag:'http://bestanimations.com/Flags/Europe/Western/Germany/german-flag-animated-gif-23.gif',name:'Saleem',country:'Germany', icon:'de',star:2 , time: '4 months', date:'23 Sep 2018', words:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla, dolorum.  amet consectetur adipisicing elit. Nulla, dolorum.'},
                {flag:'http://bestanimations.com/Flags/USA/usa-american-flag-waving-in-wind-real-close-up-animated-gif.gif',name:'Zohaib', country:'USA', icon:'us' , star:5 , time: '6 months', date:'27 Aug 2019', words:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla, dolorum. '},
                {flag:'http://bestanimations.com/Flags/Asia/bangladesh/bangladesh-flag-waving-animated-gif-7.gif',name:'Tayyab', country:'Bangladesh', icon:'bd', star:4 , time: '7 months', date:'10 Sep 2019', words:'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Nulla, dolorum. amet consectetur adipisicing elit. Nulla, dolorum.'},
            ],
        }
    },
}
</script>
<style>
    .feedback {
    float: left;
    width: 100%;
    margin: 20px auto;
    padding: 0;
}
.coment {
    float: left;
    width: 100%;
}
.coment-box {
    background: #f3f6f9 none repeat scroll 0 0;
    border-left: 7px solid #3c8dbc;
    border-radius: 4px;
    float: left;
    margin: 5px 10px;
    overflow: hidden;
    padding: 10px 150px 8px 90px;
    position: relative;
    width: 97%;
}
.coment-box:nth-child(even) {
    float: right;
    width: 95%;
    border-color:  #97be2e;
}
.coment .author-image {
    border: 3px solid #97be2e;
    border-radius: 80px;
    height: 70px;
    left: 10px;
    overflow: hidden;
    position: absolute;
    top: 10px;
    width: 70px;
}
.coment .rating-section {
    overflow: hidden;
    position: absolute;
    right: 0;
    top: 8px;
    width: 120px;
}
.coment .rating-section .rating {
    color: #ffd800;
    padding: 0;
}
.coment .rating-section .rating i {
    padding: 1px;
    font-size: 18px;
}

.coment .description {
    float: left;
    width: 95%;
    margin: 0 auto;
}
.coment .title {
    background: rgba(0, 0, 0, 0) none repeat scroll 0 0;
    min-height: 70px;
    text-align: left;
}
.related-ser .title {
    margin-bottom: 15px;
}
.coment-box .title h3 {
    font-size: 18px;
    font-weight: 500 !important;
    margin: 13px 0 0;
    color: #3c3c3c;
    text-transform: capitalize;
    font-family: 'Raleway', Arial, Helvetica, sans-serif;
}
.coment h3 .flag-icon {
    margin-left: 40px;
    font-size: 13px;
    top: -2px;
}
.flag-icon {
    margin-right: 5px;
}
.flag-icon-in {
    background-image: url(/flags/4x3/pk.svg);
}

.coment-box .title h3 small {
    color: #222222;
    font-size: 92%;
    margin-left: 0px;
    position: relative;
    text-transform: uppercase;
    top: 1px;
}
.coment-box .title p {
    color: #666666;
    font-weight: 100 !important;
    font-size: 14px;
    line-height: 20px;
        font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
}
.time > p, .date {
    font-size: 15px;
    line-height: 1.5;
    margin: 0;
}
.date {
    position: relative;
    width: 154px;
}
.time > p, .date {
    font-size: 15px;
    line-height: 1.5;
    margin: 0;
}
.related-ser .title > h2 {
    color: #414141;
    font-size: 24px;
    margin: 13px 0;
    text-align: center;
}
</style>