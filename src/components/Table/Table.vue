<template>
  <table class="table-auto">
    <TableHead/>

    <tbody>
      <TableRow
      v-for="lineup in festival.lineup"
      :lineup="lineup"
      />
    </tbody>

  </table>
</template>

<script lang="ts" setup>
import TableHead from './TableHead.vue'
import TableRow from './TableRow.vue'
</script>

<script lang="ts">
export default {
  props: {
    festival: {
      default: null,
      type: Object,
    }
  }
}
</script>