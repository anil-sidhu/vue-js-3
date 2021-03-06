<template>
<h2>User Component</h2>
<button v-on:click="getUser(userName)" >Send User Name to Parent</button>
</template>

<script>
export default {
    name: "User",
    data() {
        return {
            userName: "Peter"
        }
    },
    props:{
        getUser:Function
    }
}
</script>
