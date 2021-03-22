<template>
<h1>Teleport components</h1>
<teleport to="#footer">
<Footer />
</teleport>
</template>

<script>
import Footer from './Footer.vue';
export default {
    name: "Home",
    components:{
        Footer
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
