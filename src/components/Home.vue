<template>
<h1>For Loop in Vue js</h1>
<ul>
    <li v-for="item in technology" :key="item">
        {{item}}
    </li>
</ul>
<br /><br />
<ul>
    <li v-for="item in users" :key="item.name">
        User name is : {{item.name}} and Email is : {{item.email}}
    </li>
</ul>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            technology: [
                "java",
                "php",
                "node",
                "html",
                "asp"
            ],
            users: [{
                    name: 'anil',
                    email: 'anil@test.com'
                },
                {
                    name: 'sam',
                    email: 'sam@test.com'
                },
                {
                    name: 'peter',
                    email: 'peter@test.com'
                }
            ]
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
