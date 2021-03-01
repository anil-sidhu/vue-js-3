<template>
<h2>{{name}}</h2>
<h2>{{data.email}}</h2>
<button v-on:click="getData()">Click Me</button>

</template>

<script>
export default {
    name: 'Child',
    props: {
        name:String,
        data:Object,
        getData:Function,
    }
}
</script>
