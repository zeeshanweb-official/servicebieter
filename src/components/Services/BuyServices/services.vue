<template>
<div class="row">
    <appService v-for="service in services" :key="service.index" :service="service"></appService>
</div>
</template> 
<script>
import Service from './service'
export default {
    components:{
        appService:Service
    },
    data() {
        return {
            services:[
          {
            id:1,
            title:'Awesome Villa',
            address:'gulistan Colony SHahkot',
            image:'r-property-img.jpg',
            price:"$450",
            stars:4,
    
          },
          {
            id:2,
            title:'Good Thing',
            address:'gulistan Colony no 2 Faisalabad',
            image:'blog-full-4.jpg',
            price:"$400",
            stars:3
          },
          {
            id:3,
            title:'Very Nice Home',
            address:'Housing Society Faisalabad',
            image:'blog-full-5.jpg',
            price:"$400",
            stars:3
          },
          {
            id:4,
            title:'Very Good House',
            address:'Mustafaabad Housing Society Faisalabad',
            image:'blog-full-4.jpg',
            price:"$405",
            stars:2
          },
          {
            id:5,
            title:'Very Good House',
            address:'Mustafaabad Housing Society Faisalabad',
            image:'blog-full-3.jpg',
            price:"$405",
            stars:2
          },
          {
            id:6,
            title:'Very Good House',
            address:'Mustafaabad Housing Society Faisalabad',
            image:'blog-full-5.jpg',
            price:"$405",
            stars:2
          },
          
      ]  
        }
    },
}
</script>