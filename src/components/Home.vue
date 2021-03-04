<template>
<h1>CSS binding</h1>
<h2 class="staticClass" :class="adjustStyle">Home Component</h2>
<button v-on:click="colorfull=!colorfull">Apply Style</button>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            colorfull: false
        }
    },
    computed: {
        adjustStyle() {
            return {
                green: this.colorfull,
                err: true,
                other: false
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}

.green {
    background-color: green;
    width: 200px;
    padding: 10px;
    color: #fff
}

.err {
    color: red
}

.other {
    font-size: 70px
}
</style>
