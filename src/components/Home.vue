<template>
<h1>Form Modifiers</h1>
<input type="number"  v-model.number.lazy="item" />
<h2> Item is:{{item}}</h2>
<h2> Item is:{{typeof item}}</h2>

</template>

<script>
export default {
    name: "Home",
    data()
    {
        return {
            item:''
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
