<template>
  <section id="about" class="about-section d-flex align-center mb-16">
    <v-container class="col-2">
      <v-row
      class="align-center about-sects"
      >
        <v-col class="col-3">
          <g-image alt="profpic" src="~/img/prof2.jpg" 
          class="profimage elevation-10 rounded-circle"
          />
        </v-col>
        <v-col class="col-3">
          <v-card
          class="align-center v-sheet--shaped header-sub"
          :elevation="14"
          >
            <v-card-title
            class="blue-grey--text text--darken-2 font-weight-bold text-h5"
            >
            Hi, I'm Giorgos
            </v-card-title>
            <v-card-subtitle class="blue-grey--text text--darken-2">
              Someday I'm going to be a real software developer
              </v-card-subtitle>
            <v-card-subtitle>
              Github: <a href="https://github.com/Tsiroto" class="blue-grey--text">Tsiroto</a>
            </v-card-subtitle>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.about-section {
  background: rgb(22,147,180);
  background: -moz-linear-gradient(120deg, rgba(22,147,180,1) 0%, rgba(47,79,132,1) 100%);
  background: -webkit-linear-gradient(120deg, rgba(22,147,180,1) 0%, rgba(47,79,132,1) 100%);
  background: linear-gradient(120deg, rgba(22,147,180,1) 0%, rgba(47,79,132,1) 100%);
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#1693b4",endColorstr="#2f4f84",GradientType=1);
  height: 100vh;
  background-image: url('https://assets.codepen.io/3765537/bak.jpg');
  background-attachment: fixed;
  clip-path: ellipse(100vw 98vh at 50% 0%);
}
.about-sects {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: auto;
}
.about-sects * {
  min-width: 360px;
  margin: 12px 20px;
}
.profimage {
  max-width: 100%;
  height: auto;
  margin: auto;
}
.header-sub {
  background-color: #b2ebf2f0;
}
</style>