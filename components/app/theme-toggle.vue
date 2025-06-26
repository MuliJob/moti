<script setup lang="ts">
const colorMode = useColorMode();

const isDark = computed({
  get() {
    return colorMode.value === "halloween";
  },
  set(value: boolean) {
    colorMode.preference = value ? "halloween" : "silk";
  },
});
</script>

<template>
  <label class="swap swap-rotate mx-4">
    <input v-model="isDark" type="checkbox">
    <Icon class="swap-on" name="ic:outline-wb-sunny" size="24" />
    <Icon class="swap-off" name="ic:baseline-dark-mode" size="24" />
  </label>
</template>
