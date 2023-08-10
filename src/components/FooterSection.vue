<template>
  <v-footer class="px-1 bg-amber-accent-1">
    <v-row>
      <v-col class="text-center" cols="12">
        <div class="">
          <strong>Get connected with us on social networks!</strong>

          <v-spacer></v-spacer>

          <v-btn
            v-for="icon in icons"
            :key="icon.name"
            class="mx-4"
            :icon="icon.name"
            variant="plain"
            size="small"
          ></v-btn>
        </div>
      </v-col>
      <v-col cols="12">
        <div class="px-4 py-2 text-center w-100">
          {{ new Date().getFullYear() }} — <strong>Like Computer</strong>
        </div>
      </v-col>
    </v-row>



  </v-footer>
</template>

<script>
export default {
  data: () => ({
    icons: [
      {
        name: 'mdi-facebook',
        link: 'https://www.facebook.com/kumar.sanjel1'
      },
      {
        name: 'mdi-gmail',
        link: ''
      }
    ],
  }),
}
</script>

<style scoped>

</style>
