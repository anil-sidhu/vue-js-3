<template>
<h1>Pass Data to child Component</h1>
<Child :name="name" :data="user" :getData="getData" />
</template>

<script>
import Child from './Child.vue'
export default {
    name: "Home",
    components: {
        Child
    },
    data() {
        return {
            name: 'bruce',
            user: {
                name: 'bruce',
                email: 'bruce@test.com'
            }
        }
    },
    methods: {
        getData() {
            alert("Function called")
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
