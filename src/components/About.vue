<template>
  <section id="about">
    <v-container>
      <v-row>
        <v-col sm="6">
          <g-image alt="Example image" src="~/img/prof1.jpg" width="350" />
        </v-col>
        <v-col sm="6" class="d-flex flex-column justify-center">
          <h1>Hi, I'm Giorgos</h1>
          <div>
            <p>Someday I'm going to be a real software developer ...</p>

            <p>YouTube Channel: <a href="https://youtube.com/">Chiroto</a></p>

            <p>Github: <a href="https://github.com/chiroto">Chiroto</a></p>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
.g-image {
  border-radius: 100%;
  margin-left: 20px;
}
</style>