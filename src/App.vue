<template>
  <h1>User's Data</h1>
  <ul class="item" v-for="item in list" :key="item.id">
  <li>{{item.id}}</li>
  <li>{{item.email}}</li>
  <li>{{item.first_name}}</li>
  <li> <img :src="item.avatar" /> </li>
  </ul>
</template>

<script>
import axios from "axios"
export default {
  name: "App",
  data()
  {
      return {
          list:[]
      }
  },
  async  mounted()
  {
      let result = await axios.get("https://reqres.in/api/users?page=1");
      console.warn(result.data.data)
      this.list=result.data.data
  }

};
</script>

<style>
.item{
display:flex
}
.item img{
  width:50px;
}
.item li{
  display: inline-block;
    border: 1px solid;
    width: 180px;
    text-align: center;
    padding: 5px;
}
</style>
