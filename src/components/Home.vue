<template>
<h1>beforeMount and mounted {{name}}</h1>
</template>

<script>
export default {
    name: "Home",
    data() {

        return {
            name: 'Anil'
        }
    },
    beforeMount()
    {
        console.warn("beforeMount",this.$el)
    },
     mounted()
    { 
        console.warn("mounted",this.$el)
    },


}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
