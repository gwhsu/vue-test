<template>
    <h3> event attr</h3>
    <button @click="addCount"> Add </button>
    <p @click="getName(item)" v-for="(item, index) in names" :key="index">{{ item }}</p>
</template>

<script>

export default{
    data(){
        return{
            names: ["Riot", "Blizzard", "123"]
        }
    },
    methods:{
        getName(name){
            console.log(name)  
        }
    }

}
</script>
