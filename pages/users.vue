<template>
        <div>
        <nuxt-link to="/">Home</nuxt-link>
        <input type="text" v-model="userId">
        <button @click="onLoadUser">Load user</button>
        <p>The above will push() the input to the $router that is accepted as the id in _id folder</p>

        <nuxt-child />
    </div>
</template>


<script>
    export default {
       data(){
           return {
               userId: ''
           }
       } ,
       methods: {
           onLoadUser(){
               this.$router.push('/users/' + this.userId)
           }
       },
       layout: 'users'
    }
</script>