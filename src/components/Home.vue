<template>
<h1>Email : {{email}}</h1>
<h1>Name : {{getName("Sidhu")}}</h1>
<h1>Data : {{getData("Bruce").email}}</h1>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            email: "anil@test.com",
        }
    },
    methods: {
        getName(name) {
            return name;
        },
        getData() {
            return {
                name: "anil",
                email: this.email
            }
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
