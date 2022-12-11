<template>
  <v-card>
    <v-card-title>
      POSTS - The Vue.js way
    </v-card-title>
    <v-card-text>
      <v-card>
        <ul>

          <li v-for="post in posts" :key="post.id">
            {{post.title}}
          </li>
        </ul>

      </v-card>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      posts: [
        {id: 1, title: 'With no sense'},
        {id: 2, title: 'With no strawberries'},
      ]
    }
  },
  // async asyncData({$axios}) {
  
  //   const {data: posts} = await $axios.get('https://jsonplaceholder.typicode.com/todos')
  //   console.log('data: ', posts[0], new Date().toLocaleString())
  //   return {posts}
  //   // return {
  //   //   posts
  //   // }
  // }
}
// import axios from 'axios'
// export default {
//   data() {
//     return {
//       posts: []
//     }
//   },
//   async mounted() {
//     const { data } = await axios.get('https://jsonplaceholder.typicode.com/todos')
//     this.posts = data;
//     console.log(data);
//   }
// }
</script>

<style>

</style>