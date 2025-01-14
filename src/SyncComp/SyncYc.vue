<template>

    <div>元神启动</div>
    <!-- <div>{{ data.name }}</div>
    <div><strong>{{ data.desc }}</strong></div> -->
   
   </template>
   
   <script setup lang='ts'>
   
   import { ref,reactive } from 'vue' ;
   import {axios} from '../aaxios/Aget'
   
   interface Data{
       data:{
           name:string
           desc:string
       }
   }
   
   const {data}=await axios.get<Data>('./public/data.json')
   
   </script>
   
   <style scoped>
   
   </style>