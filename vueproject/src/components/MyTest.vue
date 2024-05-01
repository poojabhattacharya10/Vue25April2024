<template>

    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
        <title>Bootstrap demo</title>
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    </head>

    <h1 v-if="check === 10">{{ heading }}</h1>
    <h2 v-else>{{ subHeading }}</h2>

    <!-- {{ x + y  }}  -->
    <!-- {{ z }} -->

    <!-- {{  students[0] }} -->
    <!-- <h2 v-for="(student, index) in students" :key="index"> {{ student }}</h2> -->

    <!-- {{ students[0].name}} -->
    <!-- <h2 v-for="(student, index) in students" :key="index"> {{ student.name }} {{ student.mobileNo}} {{  student.address }}</h2> -->

    <input type="button" value=" Click Here " @click="add()"/>

    <table class="table">
    <thead>
        <tr>
        <th scope="col">Roll No</th>
        <th scope="col">Name</th>
        <th scope="col">Mobile No</th>
        <th scope="col">Address</th>
        </tr>
    </thead>
    <tbody>
        <tr v-for="(student , index) in students" :key="index" >
        <th scope="row">{{student.rollNo}}</th>
        <td>{{student.name}}</td>
        <td>{{student.mobileNo}}</td>
        <td>{{student.address}}</td>
        </tr>
        
    </tbody>
</table>

    <!-- <h1> Welcome to learn Vue.js </h1> -->
</template>

<script>
    export default {
        name : 'MyTest',
        data(){
            return {
                heading : 'Welcome to Bharat ',
                subHeading : 'Welocme to U.P.',
                // check : false
                // check : true
                check : 10,
                x : 2,
                y : 3,
                z : 0,
                // students : [
                //     'ram' , 'rama' , 'raman' , 'ramana'
                // ]
                students :[
                    {   
                        rollNo : 1,
                        name : 'Ram',
                        mobileNo : 7894561230,
                        address : 'Lucknow'
                    },
                    {
                        rollNo : 2,
                        name : 'Shyam',
                        mobileNo : 8894561230,
                        address : 'Delhi'
                    },
                    {
                        rollNo : 3,
                        name : 'Mohan',
                        mobileNo : 9894561230,
                        address : 'Ghaziabad'
                    }
                ]
            }
        },
        methods:{
            add(){
                // alert('Clicked')
                this.z = this.x + this.y
                this.heading = 'Welcome to RD'
            }
        }
    }
</script>

<style scoped>
    h1{
        color :crimson
    }
</style>

<!-- methods :: property -->
<!-- if variables are used in methods , then use :: this.variablename -->
<!-- no local variable used in methods -->
<!-- :key="index" -->
 <!-- : represents value of index , if we remove colon then it consider simply as a string  -->