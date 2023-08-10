<template>
  <v-main>
    <v-app-bar>
      <v-app-bar-title>
        <v-img src="@/assets/images/like-logo-slogan.png" width="300" class="primary--text">
        </v-img>
      </v-app-bar-title>
      <v-spacer></v-spacer>
      <v-btn color="primary" text class="text-capitalize">
        Home
      </v-btn>
      <v-btn color="primary" text class="text-capitalize">
        Products
      </v-btn>
      <v-btn color="primary" text class="text-capitalize">
        About
      </v-btn>
    </v-app-bar>
    <router-view />
    <footer-section></footer-section>
  </v-main>
</template>

<script>
import FooterSection from "@/components/FooterSection";
export default {
  components: {FooterSection}
}
</script>
