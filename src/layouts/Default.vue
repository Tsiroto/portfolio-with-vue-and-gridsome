<template>
  <v-app>
    <v-card
    height="100%"
    class="d-none d-md-flex"
    >
      <v-navigation-drawer permanent fixed expand-on-hover>
        <v-list-item class="fixed-nav-header">
          <v-list-item-avatar>
            <img src="@/img/prof2.jpg">
          </v-list-item-avatar>
          <v-list-item-content class="fixed-nav-title">
            <v-list-item-title class="title white--text">
              Giorgos Ntoufas
            </v-list-item-title>
            <v-list-item-subtitle class="white--text">
              Software Developer
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>

        <v-divider></v-divider>

        <v-list
          dense
          nav
        >
          <v-list-item
            v-for="item in items"
            :key="item.title"
            link
            :to="`#${item.title.toLowerCase().replace(' ', '-')}`"
          >
            <v-list-item-icon>
              <v-icon class="white--text">{{ item.icon }}</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title class="white--text">{{ item.title }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
    </v-card>
    <v-main>
      <slot/>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          { title: 'About', icon: 'mdi-account-box-outline' },
          { title: 'Projects', icon: 'mdi-apps' },
          { title: 'Warning', icon: 'mdi-access-point' },
          { title: 'People', icon: 'mdi-account-alert-outline' },
          { title: 'Contact', icon: 'mdi-message-text-outline' },
        ],
        right: null,
      }
    },
  }
</script>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
html {
  scroll-behavior: smooth;
  font-family: "Segoe UI Historic", "Segoe UI", Helvetica, Arial, sans-serif;
}
.v-application {
    font-family: "Segoe UI Historic", "Segoe UI", Helvetica, Arial, sans-serif;
    letter-spacing: -0.5px;
}
.v-application--wrap {
  flex-direction: row;
}
.v-main {
  flex: 1 0;
}
.v-navigation-drawer {
  border-radius: unset;
}
.v-navigation-drawer__content {
  background: linear-gradient(270deg, #1b2735 0%, #0e0f15 100%);
}
.fixed-nav-title {
  padding: 0;
}
.fixed-nav-header {
  padding: 8px 10px;
}
/* Scrollbar  */
::-webkit-scrollbar {
  width: 20px;
}
/* Track */
::-webkit-scrollbar-track {
  box-shadow: inset 0 0 12px 1px rgb(192, 204, 245);
  /* background: #99cde559; */
}
/* Handle */
::-webkit-scrollbar-thumb {
  /* background: #2c858a; */
  background: #1b2735;
  border-radius: 2px;
}
::-webkit-scrollbar-thumb:hover {
  background: #1b2735;
  cursor: pointer;
}

</style>