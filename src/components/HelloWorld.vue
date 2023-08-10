<template>
    <v-row class="align-center text-center">
      <v-col class="pb-0" cols="12">
      <v-img
        width="100%"
        height="400"
        cover
        src="@/assets/images/hero-image.png"
      >
        <div class="mt-15 pt-15">
          <div class="mb-n1">Welcome to</div>
          <h1 class="text-h2 font-weight-bold">Like Computer</h1>
          <div class="mb-4">
            We are a tech company providing services like
          </div>
          <div>
            <v-chip outlined color="black" small label>Hardware</v-chip>
            <v-chip color="black" class="mx-2" small label>Office Setup</v-chip>
            <v-chip color="black" class="mx-2" small label>CCTV</v-chip>
            <v-chip color="black" small label>Software Development</v-chip>
          </div>
        </div>
      </v-img>
      </v-col>
    </v-row>
   <v-row class="px-4 bg-blue-accent-1">
     <v-col class=" " cols="12">
       <feature-section></feature-section>
     </v-col>
   </v-row>
 <about-me></about-me>
  <our-client></our-client>
</template>

<script>
  //
  import FeatureSection from "@/components/FeatureSection";
  import AboutMe from "@/components/AboutMe";
  import OurClient from "@/components/OurClient";
  export default {
    components: {OurClient, AboutMe, FeatureSection},
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
