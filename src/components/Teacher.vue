<template>
<h2>Teacher Name is : {{name}} </h2>
<button v-on:click="getName('anil')">Send Name</button>
</template>

<script>
export default {
    name: 'Teacher',
    props:{
        name:String,
        getName:Function
    }
}
</script>
