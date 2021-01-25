<template>
<div class="card"> 
    <h1> {{ post.title }}</h1>
    <p> {{ post.body }} </p>
</div>
</template> 

<script>
import axios from 'axios'

export default {
    data() {
      return { 
      post: {}
      }
    },

    async created () {
     const res= await axios.get('https://jsonplaceholder.typicode.com/posts/' + this.$route.params.id)
     this.post = res.data
     console.log(this.post)
    }
}
</script>

<style>

.card {
    border: 1px solid whitesmoke;
    padding: 4rem;
}

</style>