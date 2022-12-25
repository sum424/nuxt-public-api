<template>
    <div class="mt-7 max-w-sm mx-auto text-center card">
        <p class="mt-7 text-7xl font-bold">{{error.statusCode}}</p>
        <div class="mt-7 text-6xl">Ooops. </div>
        <div class="mt-7">{{error.message}}</div>
        <button class="btn my-7" @click="handleClearError">Go back</button>
    </div>
</template> 

<script setup>
defineProps(['error'])

const handleClearError = () => clearError({redirect: '/products', fatal: true})

</script>

<style scoped>

</style>