<template>
    <h2>Heloo Word</h2>
    <h1>{{ text }}</h1>
    <button @click="changeText">Ubah text</button>
</template>


<script>
export default {
    name:"Header",
    props: ["text"],
    data(){
        return{
            newText: "ini adalah text dari header.vue"
        }
    },
    methods:{
        changeText(){
            this.$emit("changeTitle", this.newText);
        },
    },
    emits: ["changeTitle"],
};
</script>

<style>


</style>