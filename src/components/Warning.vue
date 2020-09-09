<template>
  <section id="warning" class="warning-section">
    <v-container>
      <v-row>
        <v-col>
          <h1 class="text-center">5G Warning</h1>
        </v-col>
      </v-row>
      <v-row class="w-80">
        <v-col>
          <v-timeline>
            <v-timeline-item
              v-for="(year, i) in years"
              :key="i"
              :color="year.color"
              small
            >
              <template v-slot:opposite>
                <span
                  :class="`headline font-weight-bold ${year.color}--text`"
                  v-text="year.year"
                ></span>
              </template>
              <div class="py-4">
                <h2 :class="`headline font-weight-light mb-4 ${year.color}--text`">{{ year.title}}</h2>
                <div>
                  {{ year.text }}
                </div>
              </div>
            </v-timeline-item>
          </v-timeline>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
  export default {
    data: () => ({
      years: [
        {
          color: 'cyan',
          year: '2022',
          title: '5G Dominance',
          text: 'World wields under the power of the true 5G King'
        },
        {
          color: 'green',
          year: '2020',
          title: 'Reactions to 5G',
          text: 'Pacifists and religions join forces for a better tomorrow, 5G grows stronger'
        },
        {
          color: 'pink',
          year: '2016',
          title: 'The true self',
          text: '5G publicly declared responsible for the human stupidity'
        },
        {
          color: 'brown',
          year: '1990',
          title: 'A new Power is rising',
          text: '5G has been slipping in the shadows, spreading fear and headaches'
        },
        {
          color: 'orange',
          year: '860',
          title: 'Rumors',
          text: 'About an evil future technology, suspicions of human extinction'
        },
      ],
    }),
  }
</script>

<style scoped>
.warning-section {
  background-color: #F5ECEB;
}
</style>