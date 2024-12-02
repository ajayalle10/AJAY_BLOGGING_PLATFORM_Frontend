<template>
  <div v-for="blog of blogs" :key="blog.id" >

     
    <SubBlogComponent :blog=blog />

  </div>

  
</template>

<script>
import SubBlogComponent from './SubBlogComponent.vue';

export default {
  name: "BlogComponent",
  props: {
   blogs: Array
  },
  components:{
    SubBlogComponent
  },
  data() {
    return {
      // Extended description for more content
      extendedDescription: "Read more to discover insightful details about the topic and why it matters in today's context.",
    };
  },
};
</script>

<style>

</style>
