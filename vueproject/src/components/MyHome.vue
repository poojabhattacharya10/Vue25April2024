<template>

<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Bootstrap demo</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
</head>


<div class="container">
    <div class="alert bg-success my-3">
        <h4 class="text-center" style="color: white"> Create your account </h4>
    </div>
</div>


    <div class="container">
        <div class="row">
            <div class="col"></div>
            <div class="col">
                <form action="/user/signup" method="post">


                    <div class="field my-3">
                        <label for="" class="form-label">Name</label>
                        <input type="text" class="form-control" name="name" placeholder="Enter Name">
                        <!-- name :: req.body.name -->
                    </div>

                    <div class="field my-3">
                        <label for="" class="form-label">Email</label>
                        <input type="text" class="form-control" name="email" placeholder="Enter Email">
                        <!-- name :: req.body.rollNo -->
                    </div>

                    <div class="field my-3">
                        <label for="" class="form-label">Password</label>
                        <input type="password" class="form-control" name="password" placeholder="Enter Password">
                        <!-- name :: req.body.name -->
                    </div>

                    

                    <input type="submit" value="Sign Up" class="btn btn-warning my-3 w-100">

                </form>
            </div>
            <div class="col"></div>
        </div>
    </div>
  

</template>
<script>
    export default{
        name : 'MyHome',

    }
</script>