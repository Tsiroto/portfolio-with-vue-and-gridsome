<template>
  <v-app>
    <v-card
    height="100%"
    width="256"
    >
      <v-navigation-drawer permanent fixed>
        <v-list-item>
          <v-list-item-avatar>
            <img src="https://randomuser.me/api/portraits/men/81.jpg">
          </v-list-item-avatar>
          <v-list-item-content>
            <v-list-item-title class="title">
              Giorgos Ntoufas
            </v-list-item-title>
            <v-list-item-subtitle>
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
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
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
}
.v-application--wrap {
  flex-direction: row;
}
.v-main {
  flex: 1 0;
}
.v-navigation-drawer__content {
  background: #46AFB9;
}
</style>
