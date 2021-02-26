<template>
<h1>Get Checkbox & Radio Button Value</h1>
<h3>Technology</h3>
<label for="java">Java</label>
<input type="checkbox" value="java" v-model="technology" id="java" />

<label for="node">Node</label>
<input type="checkbox" value="node" v-model="technology" id="node" />

<label for="php">Php</label>
<input type="checkbox" value="php" v-model="technology" id="php" />

<br /><br />
<h3>Profession</h3>
<label for="student">Student</label>
<input type="radio" value="student" id="student" v-model="profession"  name="profession" />
<label for="developer">Developer</label>
<input type="radio" value="developer" id="developer" v-model="profession" name="profession" />
<h4>Technology : {{technology}}</h4>
<h4>I am a {{profession}}</h4>

</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            technology: [],
            profession:null
        }
    }
}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
