<template>
    <div>
  
      <header class="shadow-sm bg-white">
        <nav class="container mx-auto p-4 flex justify-between">
          <NuxtLink to="/" class="font-bold">Sum Dojo</NuxtLink>
          <ul class="flex gap-4 ">
            <!-- for making requests ajax for spa 
                - intercepts links and response when which makes quicker then response returned from server 
                  - makes present component active automatically  
            -->
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
            <li><NuxtLink to="/products" class="btn">Products</NuxtLink></li>
            <li><NuxtLink to="/products/abc" class="btn">Products AB</NuxtLink></li>
          </ul>
        </nav>
      </header>
      
      <!-- output page content -->
      <div class="container mx-auto p-4">
        <slot />
      </div>
    </div>
  </template>

<style scoped>
.router-link-exact-active {
    color: #12b488; 
}
</style>