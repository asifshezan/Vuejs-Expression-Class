<script setup>
    // const imageUrl = "https://images.unsplash.com/photo-1581952975975-08cd95a728d4?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D";
    // const alt = "A family"

    const img = {
        src: "https://images.unsplash.com/photo-1581952975975-08cd95a728d4?q=80&w=2071&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D",
        alt: "A family."
    }



</script>

<template>
    <div>
        <!-- <img v-bind:src="imageUrl" v-bind:alt="alt"> -->
                <!-- <img :src="imageUrl" :alt="alt"> -->
        <img :src="img.src" :alt="img.alt">
        <!-- <img v-bind="img"> -->

    </div>
</template>

<style scoped>

</style>