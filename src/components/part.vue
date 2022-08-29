<template>
    <input type="text" v-model="Data" />
   <h1>{{Data}}</h1>
   <ul> <li v-for="item in technology" :key="item"> {{item}} </li>
</ul>
<br /><br />
<ul><li v-for="item in users" :key="item.namme"> name : {{item.name}} and email : {{item.email}}
</li></ul>
<chld name="biruk" />
   </template>
   <script>
 import chld from './chld.vue'
   export default {
    name: 'part',
    components:{
        chld
    }, 
    data() {
       return{
          technology: [
            "php",
            "node",
            "html"
            ], 
            users: [{
                name: "nah",
                email: "nahi@test.com"
            }]

        }
    }
}
       
   </script>
   <style scoped>h1{
   color: orange
   }
   
   </style>