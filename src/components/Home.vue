<template>
<h1>Non-Props Data</h1>
<User item="some Data" name="user-cmp" />
</template>

<script>
import User from './User.vue'
export default {
    name: "Home",
    components:{
        User
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
