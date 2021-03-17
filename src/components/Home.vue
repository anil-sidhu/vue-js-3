<template>
<Child>
    <template v-slot:header>
        <h1>Peter</h1>
    </template>

    <template v-slot:main>
      
    </template>
    <template v-slot:footer>
        <button>Buy Now</button>
    </template>
</Child>
<Child>
    <template v-slot:header>
        <h1>Anil</h1>
    </template>

    <template v-slot:main>
        <p>Code Step By Step</p>
    </template>
    <template v-slot:footer>
        <button>Buy Now</button>
    </template>
</Child>
<Child>
    <template v-slot:header>
        <h1>Bhasker</h1>
    </template>

    <template v-slot:main>
        <p>Code Step By Step</p>
    </template>
    <template v-slot:footer>
        
    </template>
</Child>
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
