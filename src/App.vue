<template>
  <v-app>
    <Nav ref="nav" />
    <v-main>
      <v-container fluid class="d-flex justify-center">
        <router-view />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Nav from "@/components/Nav";
export default {
  name: "App",
  components: {
    Nav,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
.link-no-deco {
  text-decoration: none;
}
</style>
