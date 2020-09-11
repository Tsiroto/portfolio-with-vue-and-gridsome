<template>
  <section id="about" class="about-section">
    <v-container>
      <v-row
      class="align-center about-sects"
      >
        <v-col class="profimage-col">
          <g-image alt="profpic" src="~/img/prof2.jpg" 
          class="profimage"
          />
        </v-col>
        <v-col>
          <v-card
          class="align-center v-sheet--shaped"
          :elevation="6"
          >
            <v-card-title>Hi, I'm Giorgos</v-card-title>
            <v-card-subtitle>
              Someday I'm going to be a real software developer
              </v-card-subtitle>
            <v-card-subtitle>
              YouTube Channel: <a href="https://youtube.com/">Chiroto</a><br>
              Github: <a href="https://github.com/Tsiroto">Chiroto</a>
            </v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.about-section {
  background-color: #D7766C;
}
.about-sects {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto;
}
.about-sects * {
  min-width: 360px;
  max-width: 450px;
  margin: 12px 20px;
}
.g-image {
  border-radius: 100%;
}
.profimage {
  max-width: 100%;
  height: auto;
  margin: auto;
}
.profimage-col {
  max-width: 350px;
}
</style>