<template>
  <!--to way binding --> 
  <input type="text" v-model="nama">
  {{ nama }}
  <!-- <h2> Nama: {{ nama }} </h2>
  <button v-on:click="changeName">Change Name</button> -->
  <!-- data binding -->
  <!-- <a v-bind:href="url">Go to Ulya</a> -->
  <!-- <a :href="url">Go to Ulya</a> -->
</template>

<script>

export default {
  name : "App",
  data(){
    return{
      // nama: "Ulya Nafis"
      url : "https://github.com/ulyanafisa16?tab=repositories",
      nama : "naff" ,
    };
  },
  // methods:{
  //   changeName() {
  //     this.nama = "Nafisa";
  //   },
  // },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
