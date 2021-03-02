<template>
<div class="user">
    <h2>{{data.name}}</h2>
    <h2>{{data.email}}</h2>
    <button v-on:click="getData(data.name)" >Alert User Name </button>
</div>
</template>

<script>
export default {
    name: 'User',
    props: {
        data: Object,
        getData:Function,
    }
}
</script>

<style>
.user {
    background-color: skyblue;
    border-bottom: 1px solid;
    padding: 10px;
    margin-bottom: 15px;
}
</style>
