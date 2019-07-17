<template>
  <div>
   <h1 >{{testheading}}</h1>


    <input type="text" v-model="testheading">
    <button @click="gov">test</button>
  </div>
</template>

<script>

let temp={}
    export default {
        name: "test",
      beforeCreate(){
          temp['testheading']="holoow"



      },
      data(){
          return temp
      },
      methods:{

      }

    }
</script>

<style scoped>

</style>
