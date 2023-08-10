<template>
  <v-row class="px-4">
    <v-col cols="12">

    </v-col>
    <v-col
      v-for="(item, index) in myClients"
      :key="index"
      cols="3">
      {{ item.name}}
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      myClients: [
        {
          name: 'Hangout Resturatant'
        },
        {
          name: 'Hype'
        },
        {
          name: 'Manpower'
        },
        {
          name: 'School'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
