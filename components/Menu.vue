<template>
  <v-app-bar fixed app>
    <v-toolbar-title>TimeUp Delivery</v-toolbar-title>
    <v-spacer></v-spacer>
    <v-toolbar-items class="hidden-sm-and-down">
      <v-btn v-for="item in menu" :key="item.icon" :to="item.link" text>{{
        item.title
      }}</v-btn>
    </v-toolbar-items>
    <v-menu class="hidden-md-and-up">
      <v-toolbar-side-icon slot="activator"></v-toolbar-side-icon>
      <v-list>
        <v-list-tile v-for="item in menu" :key="item.icon">
          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-menu>
  </v-app-bar>
</template>

<script>
export default {
  data() {
    return {
      menu: [
        { icon: "home", title: "Home" },
        { icon: "info", title: "About app" },
        { icon: "warning", title: "How it works" },
      ],
    };
  },

  methods: {
    menuItems() {
      return this.menu;
    },
  },
};
</script>