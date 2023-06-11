<template>
  <!--conditional and looping-->
  <div v-if="products.length">
  <ul>
    <li v-for="item in products" :key="item.id">
    {{ item.title }} - {{ item.price }}
    </li>
  </ul>
</div>
<div v-else>
  <p>No data found</p>
</div>
  <!--to way binding --> 
  <!-- <input type="text" v-model="nama">
  {{ nama }} -->

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
    return {
      // nama: "Ulya Nafis"
      // url : "https://github.com/ulyanafisa16?tab=repositories",
      // nama : "naff" ,
      products:[
        {id: 1, title:"Product 1", price:3000},
        {id: 2, title:"Product 2", price:5000},
        {id: 3, title:"Product 3", price:7000},
        {id: 4, title:"Product 4", price:4000},
        {id: 5, title:"Product 5", price:8000},
        {id: 6, title:"Product 6", price:9000},
        {id: 7, title:"Product 7", price:2000}
      ]
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
