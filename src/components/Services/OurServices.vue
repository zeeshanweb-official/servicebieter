<template>
   <div class="col-sm-12 pt-4 pb-0">
              <div class="agent-property">
                <div class="row">
                  <div v-for="image in images" :key="image.index" class="col-sm-3">
                    <MyService :image="image.image"></MyService>
                  </div>
                </div>
                </div>
              </div>
</template>
<script>
import MyService from './myservice'
export default {
  data() {
    return {
  images:[
    {
      image:'01.jpg'
    },
    {
      image:'02.jpg'
    },
    {
      image:'03.jpg'
    },
    {
      image:'04.jpg'
    },
    {
      image:'05.jpg'
    },
    {
      image:'06.jpg'
    },
    {
      image:'07.jpg'
    },
    {
      image:'08.jpg'
    },
  ],
      
    }
  },
    components:{
        MyService,
    }
}
</script>