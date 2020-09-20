<template>
  <section id="people" class="people-section my-12">
    <h1 class="text-center cyan--text text--darken-3 text-h4 font-weight-bold mb-6">People I Admire</h1>
    <v-card
    max-width="900"
    class="mx-auto elevation-6"
    >

      <v-container>
        <v-row dense class="d-flex justify-center">

          <v-col
            v-for="(item, i) in items"
            :key="i"
            cols="6"
            class="ppl-col"
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

                  <v-card-actions>
                    <v-btn
                      class="ml-2 mt-5"
                      outlined
                      rounded
                      small
                    >
                      Read More
                    </v-btn>
                  </v-card-actions>
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
    name: 'People',
    data: () => ({
      items: [
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/vincent.webp',
          title: 'Artist',
          person: 'Vincent Van Gogh',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/verne.gif',
          title: 'Author',
          person: 'Jules Verne',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/tesla.gif',
          title: 'Inventor - Scientist',
          person: 'Nikola Tesla',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/bowie.gif',
          title: 'Artist',
          person: 'David Bowie',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/elon.gif',
          title: 'Entrepreneur',
          person: 'Elon Musk',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/souris.jpg',
          title: 'Author',
          person: 'Georgios Souris',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/sagan.gif',
          title: 'Author',
          person: 'Carl Sagan',
        },
        {
          color: '#1F7087',
          src: 'https://assets.codepen.io/3765537/einstein.gif',
          title: 'Actor',
          person: 'Albert Einstein',
        },
      ],
    }),
  }
</script>

<style scoped>
  .ppl-col {
    min-width: 380px;
  }
</style>