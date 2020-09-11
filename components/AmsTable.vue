<template>
  <div>
    <!-- <h1>Some header</h1> -->
    TODO: Tabelle
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
          <tr v-for="i in 8" :key="i">
            <td>keine Mängel</td>
            <td>Bohrmaschine</td>
            <td>gute Kategorie</td>
            <td>27.05.2021</td>
            <td>Sollte dringend eingesetzt werden!</td>
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

table > tbody > tr {
  @apply bg-gray-100 shadow rounded transition duration-200 cursor-pointer text-gray-900;
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
</style>

<script>
export default {}
</script>
