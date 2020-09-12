<template>
  <div
    style="box-shadow: inset 0 8px 16px 0 rgba(0, 0, 0, 0.15)"
    class="w-1/6 bg-secondary"
  >
    <div
      class="flex items-center justify-center text-text border-b border-text border-opacity-25 py-8"
    >
      <button
        class="uppercase flex space-x-2 tracking-tighter focus:outline-none hover:text-highlight rounded-md cursor-pointer transition-colors duration-200"
      >
        <span>{{ currentModule }} hinzufügen</span>
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M12 6v6m0 0v6m0-6h6m-6 0H6"
          ></path>
        </svg>
      </button>
    </div>
    <div class="text-gray-900 pt-6 pl-6">
      <h2 class="text-2xl">{{ currentModule }}</h2>
      <div class="space-y-4 mt-8">
        <PresetCard
          :active="active[0]"
          @click.native="setActive(1)"
          :count="204"
        >
          {{ currentModule }}
          <!---->
        </PresetCard>
        <PresetCard
          :active="active[1]"
          @click.native="setActive(2)"
          :count="123"
        >
          ohne Mängel
          <!---->
        </PresetCard>
        <PresetCard
          :active="active[2]"
          @click.native="setActive(3)"
          :count="32"
        >
          mit geringen Mängel
          <!---->
        </PresetCard>
        <PresetCard
          :active="active[3]"
          @click.native="setActive(4)"
          :count="54"
        >
          mit erheblichen Mängel
          <!---->
        </PresetCard>
      </div>
    </div>
  </div>
</template>

<script>
const capitalizeFirstLetter = (str) =>
  str.charAt(0).toUpperCase() + str.slice(1)

export default {
  data: () => ({
    active: [true, false, false, false],
    currentModule: '',
  }),
  created() {
    this.currentModule = capitalizeFirstLetter(this.$route.name)
  },
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
