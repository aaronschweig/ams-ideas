<template>
  <div style="max-height: calc(100vh - 88px)" class="overflow-y-scroll">
    <!-- <h1>Some header</h1> -->
    <div class="mx-8 mt-8">
      <table
        class="table-fixed w-full"
        style="border-collapse: separate; border-spacing: 0 0.75rem"
      >
        <thead class="text-left">
          <tr>
            <th>Status</th>
            <th>Bezeichnung</th>
            <th>Kategorien</th>
            <th>nächste Prüfung</th>
            <th>Anmerkung</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="i in 12" :key="i">
            <td>
              <div
                class="flex items-center pl-6 py-1 cursor-pointer transition-all ease-out delay-200 duration-200 overflow-hidden hover:pl-2 show-on-hover rounded-full hover:border hover:bg-white"
              >
                <svg
                  v-if="mockData[i % 3].status === 'keine Mängel'"
                  class="w-6 h-6 text-green-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z"
                  ></path>
                </svg>
                <svg
                  v-else-if="mockData[i % 3].status === 'geringe Mängel'"
                  class="w-6 h-6 text-orange-400"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M20.618 5.984A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016zM12 9v2m0 4h.01"
                  ></path>
                </svg>
                <svg
                  v-else
                  class="w-6 h-6 text-red-600"
                  fill="none"
                  stroke="currentColor"
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"
                  ></path>
                </svg>
                <span class="whitespace-no-wrap overflow-hidden text-xs">{{
                  mockData[i % 3].status
                }}</span>
              </div>
            </td>
            <td>{{ mockData[i % 3].bezeichnung }}</td>
            <td>{{ mockData[i % 3].kategorien }}</td>
            <td>{{ mockData[i % 3].naechstePruefung }}</td>
            <td class="text-xs">
              {{ mockData[i % 3].anmerkung }}
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style scoped>
table > thead > tr > th {
  @apply font-normal text-sm text-text;
}
table > thead > tr > th {
  @apply font-normal text-sm text-text;
}

table > tbody > tr {
  @apply bg-gray-100 shadow transition duration-200 text-gray-900 h-20;
}
table > tbody > tr:hover {
  @apply bg-gray-200;
}
table > tbody > tr > td:first-child {
  @apply px-4 py-4;
}
table > tbody > tr > td:not(:first-child) {
  @apply pr-4 py-4;
}

.show-on-hover {
  width: 100%;
}

.show-on-hover > span {
  @apply pl-0 opacity-0 transition-all duration-200 delay-200 ease-out;
}
.show-on-hover:hover > span {
  @apply pl-1 opacity-100;
}
</style>

<script>
export default {
  data: () => ({
    mockData: [
      {
        status: 'keine Mängel',
        bezeichnung: 'Bohrmaschine',
        kategorien: ['Gute Kategorie'],
        naechstePruefung: '27.05.2021',
        anmerkung: 'Sollte dringend eingesetzt werden!',
      },
      {
        status: 'geringe Mängel',
        bezeichnung: 'Leiter',
        kategorien: ['Gute Kategorie'],
        naechstePruefung: '07.10.2019',
        anmerkung: 'Der Klappmechanismus quietscht!',
      },
      {
        status: 'erhebliche Mängel',
        bezeichnung: 'Leiter',
        kategorien: [],
        naechstePruefung: '30.09.2020',
        anmerkung: '',
      },
    ],
  }),
}
</script>
