<template>
  <p>{{ product }}</p>
</template>

<script>
// import { mapState } from "vuex";

export default {
  computed: {
    product() {
      return this.$store.getters.getProductById(this.$route.params.id);
    }
  }
};
</script>

<style></style>
