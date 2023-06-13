<template>


<header class="header">
  <nav class="navbar" id="navbar">
        
        <a href="#home" class="active">Home</a>
        <a href="#about">About</a>
        <a href="#education">Education</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
        <a onclick="darkMode()"><i class='bx bx-adjust'></i></a>
        
    </nav> 
        
</header>

<section class="home" id="home">

<Header @changeTitle="ubahText" :text="text"  />

<img  alt="" src="./assets/gambar.png">
<div class="shake">
<button @click="warnDisabled">Click me</button>
<span v-if="disabled">This feature is disabled!</span>
</div>

</section >
  <!--computed properti-->
  <!-- <input type="text" v-model="cari" placeholder="Cari">
  <ul>
    <li v-for="item in cariData" :key="item.id">
    {{ item.title }} - {{ item.price }}
    </li>
  </ul> -->

  <!--conditional and looping-->
  <!-- <div v-if="products.length">
  <ul>
    <li v-for="item in products" :key="item.id">
    {{ item.title }} - {{ item.price }}
    </li>
  </ul>
</div>
<div v-else>
  <p>No data found</p>
</div> -->

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

//cara mengimport component
import Header from "@/components/Header.vue"
export default {
  name : "App",
  components: {
    Header,
  },
  data(){
    return {
      text: "ini adalah text dari data"
    };
  },
  methods:{
    ubahText(newText){
      this.text = newText;
    }
  },

};







  // data(){
  //   return {
      // cari:"",
      // // nama: "Ulya Nafis"
      // // url : "https://github.com/ulyanafisa16?tab=repositories",
      // // nama : "naff" ,
      // products:[],
        // {id: 1, title:"Product 1", price:3000},
        // {id: 2, title:"Product 2", price:5000},
        // {id: 3, title:"Product 3", price:7000},
        // {id: 4, title:"Product 4", price:4000},
        // {id: 5, title:"Product 5", price:8000},
        // {id: 6, title:"Product 6", price:9000},
        // {id: 7, title:"Product 7", price:2000}
     
    // };
  
  // methods:{
  //   changeName() {
  //     this.nama = "Nafisa";
  //   },
  // },

  //lifecycle and Hooks
  // beforeCreate(){
  //   console.log('Before Create')
  // },

  // componen computed
  // created(){
  //   this.products = [
  //       {id: 1, title:"Product 1", price:3000},
  //       {id: 2, title:"Product 2", price:5000},
  //       {id: 3, title:"Product 3", price:7000},
  //       {id: 4, title:"Product 4", price:4000},
  //       {id: 5, title:"Product 5", price:8000},
  //       {id: 6, title:"Product 6", price:9000},
  //       {id: 7, title:"Product 7", price:2000},
  //     ];
  // },
  // computed:{
  //   cariData(){
  //      return this.products.filter((item)=>{
  //       return item.title.match(this.cari);
  //      });
  //   }
  // }


  // // beforeMount(){
  // //   console.log('Before Mount')
  // },
  // mounted(){
  //   console.log('Mounted')
  // },

</script>

<style >
*{
    margin:0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    scroll-behavior: smooth;
    font-family: 'poppins', sans-serif;
}

.header{
    position: fixed;
    top:0;
    left:0;
    width: 100%;
    padding: 2rem 9%;
    background-color: rgb(154, 106, 47);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.navbar a{
    font-size: 1.7rem;
    color: var(--text-color);
    margin-left: 4rem;
    transition: .3s;
}

section{
    min-height: 100vh;
    padding: 10rem 9% 2rem;
}
.shake {
  display: inline-block;
    padding:  1rem 2.8rem;
    background-color: rgb(41, 142, 142);
    border-radius: 5rem;
    box-shadow: 2 4 1rem var(--main-color);
    font-size: 1.6rem;
    color: var(--second-bg-color);
    letter-spacing: .2rem;
    font-weight: 900;
    transition: .5s ease;
}



</style>
