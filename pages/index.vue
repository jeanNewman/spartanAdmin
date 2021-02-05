<template>

</template>

<script>
    export default {
        mounted()
        {
          if(this.$auth.loggedIn){
            this.$router.push('/dashboard');
            console.log(`entro aqui con: ${this.$auth.loggedIn}`)
          }
          else
            this.$router.push('/login');
        }
    }
</script>

<style scoped>

</style>
