<template>
<h1>{{text}}</h1>
<div v-html="tag + tag2 + tag3">
</div>
</template>

<script>
export default {
    name: "Home",
    data()
    {
        return {
            text:"anil sidhu",
            tag:"<h2>Anil Sidhu</h2>",
            tag2:"<h2>Peter</h2>",
            tag3:"<h2>Burce</h2>",


        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
