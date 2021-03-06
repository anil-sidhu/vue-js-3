<template>
<h1>User Name : {{name}}</h1>
<User :getUser="getUserName" />
</template>

<script>
import User from './User.vue'
export default {
    name: "Home",
    data() {
        return {
            name: ''
        }
    },
    components: {
        User
    },
    methods: {
        getUserName(name) {
            this.name = name
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
