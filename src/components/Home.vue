<template>
<Child></Child>
<Child><h1>Peter</h1></Child>



</template>

<script>
import Child from './Child.vue'
export default {
    name: "Home",
    components: {
        Child
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
