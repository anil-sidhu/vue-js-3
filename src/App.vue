<template>
<img alt="Vue logo" src="./assets/logo.png">
<HelloWorld msg="" />
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

