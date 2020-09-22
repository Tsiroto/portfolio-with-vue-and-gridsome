<template>
  <section id="about" class="about-section d-flex align-center mb-16">
    <v-container>
      <v-row
      class="about-sects"
      >
        <!-- <v-col class="col-3">
          <g-image alt="profpic" src="~/img/prof2.jpg" 
          class="profimage elevation-10 rounded-circle"
          />
        </v-col> -->
        <v-col class="col-2 ">
            <v-spacer></v-spacer><h1 class="about-title text-center align-end">Giorgos Ntoufas</h1>
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
.about-title {
  color: #6e18f3;
  padding: 40px;
  filter: drop-shadow(-3px -3px 2px rgba(255, 255, 255, 0.3))
    drop-shadow(5px 5px 5px rgba(0, 0, 0, 0.2))
    drop-shadow(15px 15px 15px rgba(0, 0, 0, 0.2));
}
/* .about-sects * {
  min-width: 360px;
  margin: 12px 20px;
} */
.profimage {
  max-width: 100%;
  height: auto;
  margin: auto;
}
.header-sub {
  background-color: #b2ebf2f0;
}
</style>