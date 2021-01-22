<template>
  <v-container fluid class="navbar">
    <v-row class="align-center justify-space-between">
      <div class="heading">Auth App</div>
      <div>
        <v-btn v-if="!isLoggedIn">Login</v-btn>
        <v-btn v-else>Logout</v-btn>
      </div>
    </v-row>      
  </v-container>
</template>

<script>
export default {
    name: 'Navbar',
    data(){
        return {
            isLoggedIn: false,
        }
    }
}
</script>

<style scoped>
.navbar{
    background-color: #2d3436 !important;
    border-radius: 5px;
    padding: 25px;
}
</style>