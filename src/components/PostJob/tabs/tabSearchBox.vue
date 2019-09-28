<template>
<div>
    <multiselect v-model="value" 
    tag-placeholder="Add this as new tag" 
    placeholder="Click to add" 
    label="name" track-by="code" 
    :options="options" 
    :multiple="true" 
    :taggable="true" 
    @tag="addTag"
    :searchable="false"
    
    ></multiselect>
    <template slot="singleLabel" slot-scope="props">
        <input type="checkbox" name="checkbox" :value="props.options.name" :id="props.option.name">
    </template>
</div>
</template>
<script>
import Multiselect from 'vue-multiselect'
export default {
    data() {
        return {
             value: [
                    { name: 'Javascript', code: 'js' }
                  ],
                options: [
                    { name: 'Vue.js', code: 'vu' },
                    { name: 'Javascript', code: 'js' },
                    { name: 'Open Source', code: 'os' }
                    ]
        }
    },
    methods: {
            addTag (newTag) {
            console.log('tag made')
            const tag = {
                name: newTag,
                code: newTag.substring(0, 2) + Math.floor((Math.random() * 10000000))
            }
            this.options.push(tag)
            this.value.push(tag)
            }
  },
  components:{
      Multiselect,
  }
}
</script>
<style>
    .multiselect__tag {
        background-color: transparent;
        color: gray;
        border: 1px solid gray;
    }
    .multiselect__option--selected.multiselect__option--highlight {
        background-color: transparent;
        font-weight: 600;
        color: gray !important;
    }
    .multiselect__tag-icon{
        background-color: transparent;
    }
    .multiselect__option--highlight {
    background: none;
    color: gray;
}
.multiselect__option.multiselect__option--highlight::after{
background-color: transparent !important;

        color: gray;
}
</style>