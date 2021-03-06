<template>
<h1>Ref in Vue js 3</h1>
<input type="text" ref="input" />
<button v-on:click="getData" >Click Me</button>
</template>

<script>
export default {
    name: "Home",
    methods:{
        getData()
        {
            // this.$refs.input.focus();
            // this.$refs.input.value="code step by step";
            // this.$refs.input.style.color="red"
            console.warn(this.$refs.input.value)


        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
