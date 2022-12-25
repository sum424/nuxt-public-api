<template>
    <div>
  
      <header class="shadow-sm bg-white">
        <nav class="container mx-auto p-4 flex justify-between">
          <NuxtLink to="/products" class="font=bold">Sum Dojo Merchandise</NuxtLink>
          
        </nav>
      </header>
      
      <!-- output page content -->
      <div>
        <slot />
      </div>

      <footer class="container mx-auto p-4 flex justify-between border-t-2">
        <ul class="flex gap-4">
            <!-- for making requests ajax for spa 
                - intercepts links and response when which makes quicker then response returned from server 
                  - makes present component active automatically  
            -->
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
            <li><NuxtLink to="/products">Products</NuxtLink></li>
          </ul>
      </footer>
    </div>
  </template>

<style scoped>
.router-link-exact-active {
    color: #12b488; 
}
</style>