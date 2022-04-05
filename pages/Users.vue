<template>
  <div>
    <NavbarUsers />
    <Form/>
  </div>
</template>

<script>
import NavbarUsers from "@/components/NavbarUsers";
import Form from "@/components/Form"
export default {
  name: "users",
  components: {
      NavbarUsers,Form
    }
};
</script>