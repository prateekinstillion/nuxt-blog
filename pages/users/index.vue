<template>
  <div>
      <input type="text" v-model="userId">
      <button @click="onLoadUser">Load User</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userId: null
    };
  },
  components: {
  },
  methods: {
    onLoadUser() {
      this.$router.push(`/users/${this.userId}`);
    }
  }
  // To add a different layout
  // layout: "users"
};
</script>
