<template>
<img alt="Vue logo" src="./assets/logo.png">
<HelloWorld msg="Event in vue js 3" />
<Home />

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue'

export default {
    name: 'App',
    components: {
        HelloWorld,
        Home
    }
}
</script>

