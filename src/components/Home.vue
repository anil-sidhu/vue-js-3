<template>
<h1>Computed Property {{dollors}} </h1>
<h2>{{getResult}}</h2>
<h2>{{getData()}}</h2>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            dollors: 100,
            rupeeVal: 70,
            discount: 10,
        }
    },
    methods: {
        getData() {
            return (this.dollors * this.rupeeVal) - this.discount

        }
    },
    computed: {
        getResult() {
            return (this.dollors * this.rupeeVal) - this.discount
        }
    }

}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
