<template>
  <div
    class="max-w-[95vw] md:max-w-[90vw] 2xl:max-w-7xl mx-auto px-4 sm:px-6"
    :class="[addTopBottomPadding ? 'py-10 lg:py-20' : '']"
  >
    <slot />
  </div>
</template>

<script setup lang="ts">
const props = defineProps({
  addTopBottomPadding: {
    type: Boolean,
    default: true,
  },
});
</script>