<template>
  <table  
  class="table-auto w-full lg:w-1/2 relative">
    <TableHead/>

    <tbody class="">
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