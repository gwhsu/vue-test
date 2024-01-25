<template>
    <h3> Event Modifier</h3>
    <a @click.prevent="clickHandle" 
    href="https://www.google.com.tw/?hl=zh_TW"> Here </a>
    <div @click="clickDiv">
        <p @click="clickP">Test Bubble</p>
    </div>
</template>

<script>

export default{
    data(){
        return{
            names: ["Riot", "Blizzard", "123"]
        }
    },
    methods:{
        clickHandle(e){
            console.log("Click ! ")
        },
        clickDiv(){
            console.log("DIV")
        },
        clickP(){
            console.log("P")
        }
    }
}
</script>
