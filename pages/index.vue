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
