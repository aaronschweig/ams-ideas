<template>
  <li
    class="flex gap-4 p-4 hover:bg-gray-200 hover:text-highlight rounded-md cursor-pointer transition-colors duration-200 flex-wrap"
    :class="{
      'text-highlight': activated,
    }"
  >
    <slot name="icon" />
    <slot />
  </li>
</template>

<script>
export default {
  props: {
    activated: {
      type: Boolean,
      default: false,
    },
  },
}
</script>
