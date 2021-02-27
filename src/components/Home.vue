<template>
<h1 v-if="show"> Condtions in Vue js</h1>
<h1 v-else> else part in Vue js</h1>

<button v-on:click="show=!show" >Click ME</button>


</template>

<script>
export default {
    name: "Home",
    data()
    {
        return {
            show:true
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
