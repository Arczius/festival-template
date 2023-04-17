<template>
  <tr
  v-if="lineup !== null"
  >
    <td>{{ lineup.time }}</td>
    <td>{{ lineup.stage }}</td>
    <td>{{ lineup.artist }}</td>
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