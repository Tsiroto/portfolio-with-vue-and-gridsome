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
.v-navigation-drawer__content {
  background: rgb(28,107,132);
  background: -moz-linear-gradient(270deg, rgb(28 107 132 / 1) 0%, rgba(22,147,180,1) 100%);
  background: -webkit-linear-gradient(270deg, rgb(28 107 132 / 1) 0%, rgba(22,147,180,1) 100%);
  background: linear-gradient(270deg, rgb(28 107 132 / 1) 0%, rgba(22,147,180,1) 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#1c6b84",endColorstr="#1693b4",GradientType=1);
  background: linear-gradient(270deg, #2c858a 0%, #46c0c5 100%);
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
  box-shadow: inset 0 0 12px 1px rgb(168, 191, 206);
  /* background: #99cde559; */
}
/* Handle */
::-webkit-scrollbar-thumb {
  background: #2c858a;
  border-radius: 8px;
}
::-webkit-scrollbar-thumb:hover {
  background: #1a4d50;
}
</style>
