<template>
  <div class="container mx-auto">
    <p>
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
    </p>
    <router-view></router-view>
    <!-- <h2 class="font-bold text-red-500">{{msg}}</h2>
    <div v-for="course in courses" class="shadow p-4 mb-4 border border-gray-200">
      <h2>{{ course.name }}</h2>
      <p>{{ course.description }}</p>
    </div>
    <button @click="test">Test</button> -->
  </div>

</template>

<script>
export default{
  name:'App',
  data(){
    return {
      msg:'Welcome to vuejs app',
      courses:[
        {
          id:1,
          name:'React',
          description:'Hello React',
          price:300
        },
        {
          id:2,
          name:'VueJs',
          description:'Hello Vue',
          price:200
        },
        {
          id:3,
          name:'Angular',
          description:'Hello Angular',
          price:100
        }
      ]
    }
  },
  methods:{
    test(){
      this.msg = 'changed'
      console.log("Test")
    }
  }
}
</script>