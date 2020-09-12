<template>
  <div>
    <h1 class="text-6xl">HOME</h1>
  </div>
</template>

<script>
export default {
  data: () => ({
    active: [true, false, false, false],
  }),
  methods: {
    setActive(item) {
      this.active = this.active.map((a, idx) => {
        if (idx === item - 1) {
          return true
        }
        return false
      })
    },
  },
}
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
