<template>
 <div>
       <h1>Posts</h1>
     <post 
     v-for="post of posts"
     :key = "post.id"
     :name= "post.title" 
     :id="post.id"
     />    
 </div>
    

    
</template>

<script>
import axios from 'axios'
import Post from '../../components/Post'

export default {
    components: {
        Post
    },
    data() {
        return  {
            posts : []
        }
    },
    async created() {
     const res= await axios.get('https://jsonplaceholder.typicode.com/posts')
     this.posts = res.data
    }
}
</script>