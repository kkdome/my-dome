<template>
  <img alt="Vue logo" src="./assets/dome.jpg">
  <h1>{{name}}</h1>
  <h1>{{lastname}}</h1>
  <h1>{{nickname}}</h1>
  <h1>{{age}}</h1>
  <h1>{{tel}}</h1>
  <h1>{{room}}</h1>
  <h1>{{major}}</h1>
  <h1>{{school}}</h1>
  <h2>{{ getFullname() }}</h2>
  <h3>{{ hobby }}</h3>
  <h4>{{ profile }}</h4>
  <ul>
    <li>{{ hobby[0] }}</li>
    <li>{{ hobby[1] }}</li>
  </ul>
  <ul>
    <li>{{ profile.gender }}</li>
    <li>{{ profile.weight }}</li>
    <li>{{ profile.hight }}</li>
    <li>{{ profile.status }}</li>
  </ul>
</template>

<script>

export default {
  name: 'App',
  data(){
  return{
    name:"Eakkawee",
    lastname:"Sriwichai",
    nickname:"Dome",
    age:"20",
    tel:"0639239948",
    room:"IT.5102",
    major:"Information Technology",
    school:"Polytechniclannachiangmai",
    hobby: ["เล่นเกม","นอน","ดูหนัง","ฟังเพลง","กินข้าว"],
    profile: { gender: "male", weight: 50, hight: 170, status: false}
  }
},
 methods: {
  getFullname() {
    return this.firstname + this.lastname
  }
 }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
