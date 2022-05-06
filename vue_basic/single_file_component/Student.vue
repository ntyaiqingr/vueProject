<template>
    <div class="demo">
        <h2>Student Name: {{ studentName }}</h2>
        <h2>Student Age: {{ studentAge}}</h2>
        <button @click="showName">Click me to show student name</button>
    </div>
</template>

<script>
    export default {
        name: "Student",
        data() {
            return {
                studentName: "Nick",
                studentAge: 31
            }
        },
        methods: {
            showName(){
                alert(this.studentName)
            }
        }
    }
</script>

<style>
    .demo{
        background-color: orange;
    }
</style>