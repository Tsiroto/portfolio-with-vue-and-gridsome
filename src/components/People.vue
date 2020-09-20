<template>
  <section id="people" class="people-section my-12">
    <h1 class="text-center cyan--text text--darken-3 text-h4 font-weight-bold mb-6">People I Admire</h1>
    <v-card
    max-width="400"
    class="mx-auto"
    >
      <v-system-bar
        color="pink darken-2"
        dark
      >
        <v-spacer></v-spacer>

        <v-icon>mdi-window-minimize</v-icon>

        <v-icon>mdi-window-maximize</v-icon>

        <v-icon>mdi-close</v-icon>
      </v-system-bar>

      <v-app-bar
        dark
        color="pink"
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>People</v-toolbar-title>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-magnify</v-icon>
        </v-btn>
      </v-app-bar>

      <v-container>
        <v-row dense>

          <v-col
            v-for="(item, i) in items"
            :key="i"
            cols="12"
          >
            <v-card
              :color="item.color"
              dark
            >
              <div class="d-flex flex-no-wrap justify-space-between">
                <div>
                  <v-card-title
                    class="headline"
                    v-text="item.person"
                  ></v-card-title>

                  <v-card-subtitle v-text="item.title"></v-card-subtitle>

                  <v-card-action>
                    <v-btn
                      v-if="item.person === 'Ellie Goulding'"
                      class="ml-2 mt-3"
                      fab
                      icon
                      height="40px"
                      right
                      width="40px"
                    >
                      <v-icon>mdi-play</v-icon>
                    </v-btn>

                    <v-btn
                      v-else
                      class="ml-2 mt-5"
                      outlined
                      rounded
                      small
                    >
                      Read More
                    </v-btn>
                  </v-card-action>
                </div>

                <v-avatar
                  class="ma-3"
                  size="125"
                  tile
                >
                  <v-img :src="item.src"></v-img>
                </v-avatar>
              </div>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </section>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          color: '#1F7087',
          src: '~/img/vincent.webp',
          title: 'Artist',
          person: 'Vincent Van Gogh',
        },
        {
          color: 'primary',
          src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
          title: 'Author',
          person: 'Jules Verne',
        },
        {
          color: '#1F7087',
          src: 'https://cdn.vuetifyjs.com/images/cards/foster.jpg',
          title: 'Inventor - Scientist',
          person: 'Nikola Tesla',
        },
        {
          color: 'primary',
          src: 'https://cdn.vuetifyjs.com/images/cards/halcyon.png',
          title: 'Entrepreneur',
          person: 'Elon Musk',
        },
      ],
    }),
  }
</script>
