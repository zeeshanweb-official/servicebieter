<template>
         <div class="coment-box">
                                <div class="author-image"><img style="width: 69px;height: 65px;" :src="comment.flag" border="0" alt="animated-pakistan-flag-image-0001" /></div>
                                <div class="rating-section">
                                  <div class="rating">
                                      <i class="fa fa-star" v-for="star in comment.star" :key="star.index"></i>
                                  </div>
                                  <div class="time">
                                    <p>{{comment.time}} ago</p>
                                  </div>
                                  <div class="date">{{comment.date}}</div>
                                </div>
                                <div class="description">
                                  <div class="title">
                                    <h3>{{comment.name}}<span class="flag-icon" :class="'flag-icon-'+comment.icon"></span><small>{{comment.country}}</small>
                                    </h3>
                                    <p>{{comment.words}}</p>
                                  </div>
                                </div>
        </div>
</template>
<script>
export default {
            props:['comment']
}
</script>
<style>
    
</style>