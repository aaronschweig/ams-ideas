<template>
  <nuxt-link
    tag="li"
    :to="to"
    class="flex gap-4 p-4 hover:bg-gray-200 hover:text-highlight rounded-md cursor-pointer transition-colors duration-200 flex-wrap"
  >
    <slot name="icon" />
    <slot />
  </nuxt-link>
</template>

<style scoped>
.nuxt-link-exact-active {
  @apply text-highlight;
}
</style>

<script>
export default {
  props: {
    to: {
      type: String,
      default: '/',
    },
  },
}
</script>
