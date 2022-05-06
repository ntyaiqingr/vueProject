<template>
    <div class="demo">
        <h2>School Name: {{ schoolName }}</h2>
        <h2>School Address: {{ schoolAddress}}</h2>
        <button @click="showName">Click me to show school name</button>
    </div>
</template>

<script>
    export default {
        name: "School",
        data() {
            return {
                schoolName: "yigao",
                schoolAddress: "luoyang"
            }
        },
        methods: {
            showName(){
                alert(this.schoolName)
            }
        }
    }
    // 统一暴露
    // export {school} 
    // 默认暴露 *
    // export default school
</script>

<style>
    .demo{
        background-color: aqua;
    }
</style>