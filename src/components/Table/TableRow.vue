<template>
  <tr
  class="bg-gray-200 even:bg-gray-300"
  v-if="lineup !== null"
  >
    <td
    class="p-3 border-r-2 border-r-gray-500"
    >{{ lineup.time }}</td>
    <td
    class="p-3 border-r-2 border-r-gray-500"
    >{{ lineup.stage }}</td>
    <td
    class="p-3"
    >{{ lineup.artist }}</td>
  </tr>
</template>

<script lang="ts">
export default {
  props: {
    lineup: {
      default: null,
      type: Object,
    }
  }
}
</script>