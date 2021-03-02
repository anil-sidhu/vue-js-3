<template>
<h1>Reuse Component</h1>
<ul>
    <li v-for="item in users" :key="item.name">

        <User :data="item" :getData="getData" />
    </li>
</ul>
</template>

<script>
import User from './User.vue'
export default {
    name: "Home",
    components: {
        User
    },
    methods: {
        getData(name) {
            alert(name)
        }
    },
    data() {
        return {
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
                },
                {
                    name: 'bruce',
                    email: 'bruce@test.com'
                },

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
