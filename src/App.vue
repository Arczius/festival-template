<template>

  <main>
    <h1 
    class="text-5xl font-bold text-center pb-5"
    >Festival Schema</h1>

    <section 
    class="flex flex-col items-center pb-8"
    v-for="festival in festivals">
      <h2
      role="title"
      class="text-3xl font-bold"
      >{{ festival.Name }}</h2>
      <Table
      :festival="festival"
      />
    </section>
  </main>

</template>

<script lang="ts" setup>
import { festivals } from './timetable.json'
import Table from './components/Table/Table.vue'
</script>
