<template>

  <main>
    <h1 
    class="text-4xl font-bold"
    >Festival Schema</h1>

    <section 
    v-for="festival in festivals">
      <h2
      class=""
      role="title"
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
