<template>
    <div>
        <h1>A single user, with ID: {{ $route.params.id }}</h1>
        <p>Only shown if /users has /users/any-value</p>
    </div>
</template>

<script>
    export default {
        validate (data){
            console.log(data);
            return /^\d+$/.test(data.params.id)
        } 
    }
</script>

<style scoped>

</style>