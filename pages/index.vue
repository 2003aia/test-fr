<template>
  <div class="">
   
    <h2>Home Page <NuxtLink to="/users">пользователи</NuxtLink></h2>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
export default {
  name: "IndexPage",
  components: {
    Navbar,
  },
};
</script>

<style scoped>

</style>