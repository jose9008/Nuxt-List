<template>
<h1> Welcome to my first Nuxt Projects</h1>  
</template>

<script>
export default {
  head() {
    return {
      title : "Aplication Nuxt Post | Home",
      meta : [{
        hid : "description",
        name : "description",
        content : "Website about Post"
      }],
      htmlAttrs : {
        lang : 'en'
      }
    }
  }
} 
</script>