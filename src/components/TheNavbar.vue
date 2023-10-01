<!-- Navbar.vue -->
<template>
   <nav class="flex items-center justify-between p-4 bg-blue-500">
      <!-- Logo on the left -->
      <a @click="linkHandler" class="flex items-center cursor-pointer">
         <h5 class="text-2xl text-white p-2">El</h5>
      </a>

      <!-- Buttons on the right -->
      <div class="flex items-center">
         <a class="text-white mr-4">
            <router-link :to="{ name: 'login' }"> Login </router-link>
         </a>
         <button class="bg-white text-blue-500 px-4 py-2 rounded">
            <router-link :to="{ name: 'register' }"> Register </router-link>
         </button>
      </div>
   </nav>
</template>

<script>
export default {
   name: "Navbar",
   methods: {
      linkHandler() {
         return this.$router.push("/")
      },
   },
}
</script>

<style scoped>
/* Add any additional styles specific to this component */
</style>
