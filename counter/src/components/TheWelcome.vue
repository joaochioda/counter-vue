<template>
  <ButtonIncrease @clicked-button="increase" />
  <ButtonDecrease @clicked-button="decrease" />

  <p>Taps: {{ counter }}</p>
</template>

<script lang="ts">
import ButtonIncrease from "@/components/ButtonIncrease.vue";
import ButtonDecrease from "@/components/ButtonDecrease.vue";

export default {
  name: "TheWelcome",
  components: { ButtonIncrease, ButtonDecrease },
  methods: {
    increase() {
      this.counter++;
    },
    decrease() {
      this.counter--;
    },
  },
  data() {
    return {
      counter: 0 as number,
    };
  },
};
</script>
