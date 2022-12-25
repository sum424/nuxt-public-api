<template>
    <div>

      <h2>about</h2>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae aut modi, omnis tempore repudiandae doloremque!</p>
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Beatae aut modi, omnis tempore repudiandae doloremque!</p>
      <div class="">{{data}}</div>
    </div>
  </template>
  
  <script setup>
  const {data} = await useFetch('/api/currency/GBP')
  </script>
  
  <style>
   h2 {
      margin-bottom: 20px;
      font-size: 36px;
   }
  
   p { 
      margin: 20px 0;
   }
   
  </style>