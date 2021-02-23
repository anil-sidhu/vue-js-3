<template>
<h1>Email : {{email}}</h1>
<h1>Mobile : {{mobile}}</h1>

<h1>Name : {{getName("Anil Sidhu")}}</h1>

</template>

<script>
export default {
    name: "Home",
    data()
    {
        return {
            email:"anil@test.com",
            mobile:9999,
            getName(x)
            {
                return x;
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
