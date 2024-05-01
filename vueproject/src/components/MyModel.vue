<template>

    <head>
            <meta charset="utf-8">
            <meta name="viewport" content="width=device-width, initial-scale=1">
            <title>Bootstrap demo</title>
            <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    </head>

    <h1> Going to apply v-model </h1>

    <!-- <input type="text" class="form-control" v-model="name" placeholder="Enter Email"/>
    <h1> Name : {{ name }} </h1> -->

    <input type="text" class="form-control" v-model="p" placeholder="Enter principal"/>
    <p> principal : {{ p }} </p> 

    <input type="text" class="form-control" v-model="r" placeholder="Enter rate"/>
    <p> rate : {{ r }} </p> 

    <input type="text" class="form-control" v-model="t" placeholder="Enter time"/>
    <p> time : {{ t }} </p> 

    <h2> SI : {{  si }}</h2>

    <input type="button" value=" Calculate" class="btn btn-warning" @click="cal()"/>

</template>


<script>
    export default {
        name : 'MyModel',
        data(){
            return {
                // name : ''
                p : 0,
                r : 0,
                t: 0,
                si : 0
            }
        },
        methods : {
            cal(){
                this.si = (this.p * this.r * this.t)/100
             }
        }
    }
</script>


<style>

</style>


<!-- v-model :: two way binding -->