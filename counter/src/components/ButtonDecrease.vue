<template>
  <div>
    <button @click="doSomething">Decrease</button>
  </div>
</template>

<script>
export default {
  emits: ["clicked-button"],
  methods: {
    doSomething() {
      this.$emit("clicked-button");
      console.log("decreased");
    },
  },
};
</script>

<style scoped>
button {
  background-color: #6c1515;
  border: none;
  padding: 10px;
  border-radius: 13px;
  font-size: 15px;
  color: white;
  font-weight: 700;
  cursor: pointer;
}
</style>
