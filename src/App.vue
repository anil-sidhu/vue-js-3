<template>
<router-link to="/">Home Page</router-link> <br />
<router-link to="/login">Login Page</router-link> <br />
<router-link to="/profile/Peter">Peter's Profile Page</router-link> <br />

<router-view />
</template>

<script>
export default {
    name: 'App',
}
</script>
