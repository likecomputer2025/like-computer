<template>
  <v-row>
    <v-col class="text-h6" cols="12">
      Our Top Product and services
    </v-col>
    <v-col v-for="(topFeature, index) in topFeatures" :key="index" cols="12" md="4">
      <v-hover>
        <template v-slot:default="{ isHovering, props }">
          <v-card :variant="!isHovering ? '' : 'outlined'"  v-bind="props"
                  :flat="!isHovering ? true : false" flat rounded >
            <v-card-title>
              {{ topFeature.title}}
            </v-card-title>
            <v-card-text>
              {{ topFeature.description}}
            </v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn rounded class="text-capitalize" v-text="'Contact for more info'"></v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-hover>
    </v-col>
  </v-row>
</template>

<script>
export default {
    data () {
      return {
        topFeatures: [
          {
            title: 'CCTV Facility',
            description: 'From new CCTV installation to mantanance and upgarde. No comparmise and available in all price option.',
            image: ''
          },
          {
            title: 'Computer Repair',
            description: 'From new CCTV installation to mantanance and upgarde. No comparmise and available in all price option.',
            image: ''
          },
          {
            title: 'Network Service and parts',
            description: 'From new CCTV installation to mantanance and upgarde. No comparmise and available in all price option.',
            image: ''
          }
        ]
      }
    }
}
</script>

<style scoped>

</style>
