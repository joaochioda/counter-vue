<template>
  <div>
    <button @click="doSomething">Increase</button>
  </div>
</template>

<script>
export default {
  emits: ["clicked-button"],
  methods: {
    doSomething() {
      this.$emit("clicked-button");
      console.log("increased");
    },
  },
};
</script>

<style scoped>
button {
  background-color: #286c15;
  border: none;
  padding: 10px;
  border-radius: 13px;
  font-size: 15px;
  color: white;
  font-weight: 700;
  cursor: pointer;
}
</style>
