<template>
  <div class="list">
    <v-list flat>
      <v-list-item-group v-model="selectedItem" color="primary">
        <v-list-item v-for="(item, i) in items" :key="i">
          <router-link to="/listcontent" class="link-no-deco">
            <v-list-item-content>
              <v-list-item-title
                v-text="item.text"
                class="list-text"
              ></v-list-item-title>
            </v-list-item-content>
          </router-link>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </div>
</template>

<script>
export default {
  data: () => ({
    selectedItem: 1,
    items: [
      { text: "Judul List 1", icon: "mdi-clock" },
      { text: "Judul List 2", icon: "mdi-account" },
      { text: "Judul List 3", icon: "mdi-flag" },
      { text: "Judul List 4", icon: "mdi-clock" },
      { text: "Judul List 5", icon: "mdi-account" },
      { text: "Judul List 6", icon: "mdi-flag" },
    ],
  }),
};
</script>

<style>
.list-text {
  color: #2b6777;
  font-weight: 600;
}
</style>
