<template>
<h1>Simple Form</h1>
<p>{{form}}</p>
<form>
    <label>Email : </label>
    <input type="text" placeholder="enter email" v-model="form.email" />
    <br /> <br />

    <label>Password : </label>
    <input type="password" placeholder="enter password" v-model="form.password" />
    <br /> <br />
    <select v-model="form.country">
        <option>India</option>
        <option>USA</option>
    </select>
    <br /> <br />.
    <h3>Gender</h3>
    <label>Male : </label>
    <input type="radio" name="gender" value="male" v-model="form.gender" />
    <br /> <br />
    <label>Female : </label>
    <input type="radio" name="gender" value="female" v-model="form.gender" />
    <br /> <br />
    <h3>Technology</h3>
    <label>Java : </label>
    <input type="checkbox" value="java" v-model="form.technology" />
    <br /> <br />
    <label>.Net : </label>
    <input type="checkbox" value=".net" v-model="form.technology" />
    <br /> <br />
    <button v-on:click="login" type="button">Login</button>

</form>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            form: {
                email: '',
                password: '',
                country: '',
                gender: '',
                technology: []
            }
        }
    },
    methods: {
        login() {
            
            console.warn(this.form)
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
