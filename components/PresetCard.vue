<template>
  <div
    class="p-6 rounded-md rounded-r-none cursor-pointer transition duration-200"
    :class="{ 'bg-white my-shadow': active, 'hover:bg-gray-400': !active }"
  >
    <p class="text-4xl text-gray-900">{{ count }}</p>
    <span class="text-text text-sm">
      <slot />
    </span>
  </div>
</template>

<style scoped>
.my-shadow {
  box-shadow: -4px 4px 6px -1px rgba(0, 0, 0, 0.1);
}
</style>

<script>
export default {
  props: {
    active: {
      type: Boolean,
      default: false,
    },
    count: {
      type: Number,
      default: 0,
    },
  },
}
</script>
