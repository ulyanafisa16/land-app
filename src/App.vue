<template>

<body>
<header class="header">
  <a href="#" class="logo">ORIGINOTE</a>

  <nav class="navbar" id="navbar">
        
        <a href="#home" class="active">Home</a>
        <a href="#about">About</a>
        <a href="#education">Shop</a>
        <a href="#contact">Contact</a>
        <a onclick="darkMode()"><i class='bx bx-adjust'></i></a>
        
    </nav> 
</header>

<section class="home" id="home" >
        <div class="home-content">
            <h3>Hello, it's Me</h3>
            <h1>Originote</h1>
            <h3>Skin Health <span class="multiple-text"></span></h3>
            <p>untuk kulit sehat dan bersih</p>
                 <div class="social-media">
                    
                    <a href="https://twitter.com/nafisaa_yaa"><i class='bx bxl-twitter'></i></a>
                    <a href="https://instagram.com/theoriginote"><i class='bx bxl-instagram-alt' ></i></a>
                    <a href="https://linkedin.com/in/ulya-nafis"><i class='bx bxl-linkedin' ></i></a>
                    <a href="https://github.com/ulyanafisa16"><i class='bx bxl-github'></i></a>
                    <a href="https://codingawalannew.blogspot.com"><i class='bx bxl-blogger'></i></a>
                 </div>
                 
        </div>
        <div class="home-img">
            <img src="">
        </div>

    </section>


    <section class="skills" id="skills" >
        <h2 class="heading">What I  <span>SkinCare</span></h2>

     <div class="skills-container">
        <div class="skills-box">
            <img src="./assets/gambar3.jpg" alt="">
            <div class="skills-layer">
                <h4>ORIGINOTE</h4>
                <p>I am a well-known designer and have good skills</p>
                <a href="#"><i class='bx bx-link-external'></i></a>
            </div>
        </div>

        <div class="skills-box">
            <img src="./assets/gambar5.jpg" alt="">
            <div class="skills-layer">
                <h4>ORIGINOTE</h4>
                <p>Reading can open a window of knowledge, many things I get from reading</p>
                <a href="#"><i class='bx bx-link-external'></i></a>
            </div>
        </div>

        <div class="skills-box">
            <img src="./assets/gambar6.jpg" alt="">
            <div class="skills-layer">
                <h4>ORIGINOTE</h4>
                <p>Cooperation with people can increase our connections and networking</p>
                <a href="#"><i class='bx bx-link-external'></i></a>
            </div>
        </div>

        <div class="skills-box">
            <img src="./assets/gambar7.jpg" alt="">
            <div class="skills-layer">
                <h4>ORIGINOTE</h4>
                <p>The programming languages that I have learned are Java, HTML, Java Script and CSS</p>
                <a href="#"><i class='bx bx-link-external'></i></a>
            </div>
        </div>

        <div class="skills-box">
            <img src="./assets/gambar8.jpg" alt="">
            <div class="skills-layer">
                <h4>ORIGINOTE</h4>
                <p>I am still learning in web development to create a responsive and interactive web</p>
                <a href="#"><i class='bx bx-link-external'></i></a>
            </div>
        </div>

        <div class="skills-box">
            <img src="./assets/gambar2.jpg" alt="">
            <div class="skills-layer">
                <h4>ORIGINOTE</h4>
                <p>I like fashion first, I like to draw clothes models and like to combine various clothes</p>
                <a href="#"><i class='bx bx-link-external'></i></a>
            </div>
        </div>
    </div>
    </section>
</body>
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
  //     cari:"",
  //     nama: "Ulya Nafis"
  //     url : "https://github.com/ulyanafisa16?tab=repositories",
  //     nama : "naff" ,
  //     products:[],
  //       {id: 1, title:"Product 1", price:3000},
  //       {id: 2, title:"Product 2", price:5000},
  //       {id: 3, title:"Product 3", price:7000},
  //       {id: 4, title:"Product 4", price:4000},
  //       {id: 5, title:"Product 5", price:8000},
  //       {id: 6, title:"Product 6", price:9000},
  //       {id: 7, title:"Product 7", price:2000}
     
  //   };
  
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

body{
  background-color: rgb(102, 149, 203);
  background-image: url('./assets/gambar12.jpg');
}

.header{
    position: fixed;
    top:0;
    left:0;
    width: 100%;
    padding: 2rem 5%;
    background-color: rgb(175, 175, 206);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.navbar a{
    font-size: 1.5rem;
    color: rgb(66, 100, 131);
    margin-left: 4rem;
    transition: .3s;
}

section{
    min-height: 100vh;
    padding: 10rem 9% 2rem;
}




.home {
    display: flex;
    justify-content: left;
    align-items: center;
}

.home-img img {
    width: 35vw;
    animation: floatImage 4s ease-in-out infinite;   
}

.home-content h3 {
    font-size: 3.2rem;
    font-weight: 700;
}

.home-content h3:nth-of-type(2) {
    margin-bottom: 2rem;
}

span {
    color: rgb(169, 99, 115);
}
.home-content h1 {
    font-size: 5.6rem;
    font-weight: 700;
    line-height: 1.3;
    color: rgb(129, 160, 188);
}

.home-content p {
    font-size: 1.6rem;
    color: rgb(142, 170, 197);
    
}


.logo{
    font-size: 2.5rem;
    color: rgb(205, 143, 143);
    font-weight: 600;
    cursor: default;
}

.social-media a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background: transparent;
    border: .2rem solid var(--main-color);
    border-radius: 50%;
    font-size: 2rem;
    color: rgb(79, 100, 169);
    margin: 3rem 1rem 3rem 0;
    transition: .5s ease;
}

.social-media a:hover {
   background: var(--main-color);
   color: rgb(222, 167, 220); 
   box-shadow: 0 0 1rem var(--main-color);
}

.skills {
    background-color: rgb(115, 150, 231);
    background-image: url('./assets/gambar9.jpg');
}
.skills h2 {
   margin-bottom: 4rem; 
}
.skills-container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    align-items: center;
    gap: 2.5rem;
}
.skills-container .skills-box {
    position: relative;
    border-radius: 2rem;
    /* box-shadow: 0 0 1rem rgb(183, 202, 238);; */
    overflow: hidden;
    display: flex;
}
.skills-box img {
    width: 100%;
    transition: .5s ease;
}

.skills-box:hover img {
    transform: scale(1.1);
}
.skills-box .skills-layer {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(rgba(108, 74, 26, 0.1), var(--main-color));
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    text-align: center;
    padding: 0 4rem;
    transform: translateY(100%);
    transition: .5s ease;
}
.skills-box:hover .skills-layer {
    transform: translateY(0);
}


.skills-layer h4 {
    font-size: 3rem;
}
.skills-layer p {
    font-size: 1.6rem;
    margin: .3rem 0 1rem;
}
.skills-layer a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 5rem;
    height: 5rem;
    background-color: rgb(208, 219, 230);
    border-radius: 50%;
}
.skills-layer a i {
    font-size: 2rem;
    color: aliceblue;
}


</style>
