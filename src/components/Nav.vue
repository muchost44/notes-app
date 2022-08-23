<template>
  <v-container class="d-flex justify-center" fluid>
    <router-link
      v-for="item in items"
      :key="item"
      class="router-link mx-2 link"
      :to="item.link"
    >
      <span class="link-text"> {{ item.title }} </span>
    </router-link>
  </v-container>
</template>

<script>
export default {
  name: "Nav",

  data: () => ({
    items: [
      {
        title: "Home",
        link: "/",
      },
      {
        title: "Note",
        link: "/note",
      },
      {
        title: "List",
        link: "/list",
      },
    ],
  }),
};
</script>

<style>
.link {
  text-decoration: none;
}
.link-text {
  font-weight: 700;
  font-family: "Inter";
  color: #52ab98;
}
</style>
