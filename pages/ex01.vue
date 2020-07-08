<template>
  <div>
    <h2>Hello {{ name }}</h2>
    <h2>age {{ age }}</h2>
    <h2><input type="text" :value="name"></h2>
    <input type="text" v-model="name">
    <div><button @click="doSave">SAVE</button></div>
    <div><button @click="doMENU">MANI MENU</button></div>
    <button @click="doHOME">HOME</button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      name: "Kannathorn",
      age: 19,
    }
  },
  methods:{
    doSave(){
    console.log("DO SAVE");
    },
    doMENU(){
    this.$router.push('/menu')
    },
    doHOME(){
     this.$router.push('/ex01') 
    }
  },
}
</script>