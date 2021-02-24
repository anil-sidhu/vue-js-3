<template>
<h1 v-on:mousemove="getConsole()">Home Component </h1>
<button v-on:click="getData()">Click Me</button>
<button v-on:click="getConsole('button 2 click')">Click Me</button>
<h2>{{count}}</h2>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            count: 0
        }
    },
    methods: {
        getData() {
            this.count = this.count + 1
        },
        getConsole() {
            this.count = this.count - 1
        }
    }

}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
