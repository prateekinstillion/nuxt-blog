<template>
  <div>
    <h1>A Single User, with ID : {{ $route.params.id }}</h1>
  </div>
</template>

<script>
export default {
  validate(data) {
    console.log(data);
    const regex = new RegExp("^[0-9]+$");
    if (typeof data.params.id === "string" && !regex.test(data.params.id)) {
      return false;
    }
    return true;
  },
  layout: "users"
};
</script>

<style lang="scss" scoped>
</style>
