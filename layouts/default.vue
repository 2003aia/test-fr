<template>
  <div class="main">
    <Navbar />
    <main>
      <div class="container">
        <Nuxt />
      </div>
    </main>
  </div>
</template>
<script>
import Navbar from "@/components/Navbar";
export default {
  components: {
    Navbar,
  },
};
</script>

<style scoped>
.main {
  display: flex;
  width: 100%;
  min-width: 800px;
  justify-content: center;
}
.container {
  padding: 20px 50px 20px 50px;
  
}
main {
  width: 700px;
}
</style>