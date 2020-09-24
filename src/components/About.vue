<template>
  <section id="about" class="about-section d-flex align-end mb-14">
    <v-container>
      <v-row>
        <v-spacer></v-spacer>
        <v-col class="relative">
          <svg id="supertitle" width="400" height="68" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 400 68">
    <path d="M36,17H18.72V29H34.61v9H18.72V57h-11V8H36Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M85.2,57H72.51L64.89,44.42c-.57-1-1.11-1.81-1.64-2.56a13.42,13.42,0,0,0-1.59-1.93A6,6,0,0,0,60,38.7a4.21,4.21,0,0,0-1.9-.43h-3V57h-11V8h17.5Q79.41,8,79.42,21.35a13.71,13.71,0,0,1-.79,4.74A13,13,0,0,1,76.41,30a14.26,14.26,0,0,1-3.47,3,17.86,17.86,0,0,1-4.53,2v.14a6.65,6.65,0,0,1,2.12,1.11,14.3,14.3,0,0,1,2,1.79,23.6,23.6,0,0,1,1.83,2.21c.58.78,1.11,1.55,1.59,2.3ZM55.12,16.29V29.93H59.9a7.93,7.93,0,0,0,5.71-2.05,6.84,6.84,0,0,0,2.19-5.16q0-6.43-7.69-6.43Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M109.8,57.89q-10.51,0-17.15-6.85T86,33.18q0-11.62,6.73-18.8T110.59,7.2q10.5,0,17,6.87T134,32.19q0,11.55-6.72,18.62T109.8,57.89Zm.48-41.19a11.14,11.14,0,0,0-9.23,4.36q-3.4,4.36-3.41,11.54t3.41,11.52a11.81,11.81,0,0,0,18,.11q3.34-4.11,3.35-11.43,0-7.62-3.25-11.86A10.62,10.62,0,0,0,110.28,16.7Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M186.26,57H175.12l-20.2-30.79a46.87,46.87,0,0,1-2.46-4.07h-.14c.19,1.73.28,4.38.28,7.93V57H142.17V8h11.9l19.45,29.84c.88,1.34,1.7,2.68,2.46,4h.13a53,53,0,0,1-.27-6.73V8h10.42Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M231.89,17h-14V57H206.84V17H192.93V8h39Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M287.2,57H257.8V8h28.27v9H268.84v10.9h16v9h-16V48.08H287.2Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M339.15,57H328l-20.2-30.79a42.21,42.21,0,0,1-2.46-4.07h-.14c.18,1.73.27,4.38.27,7.93V57H295.06V8H307L326.4,37.86c.89,1.34,1.71,2.68,2.46,4H329a53,53,0,0,1-.27-6.73V8h10.42Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
    <path d="M350.36,57V8h17.36q26.11,0,26.12,23.89,0,11.46-7.13,18.29t-19,6.83Zm11-40V48.08h5.47q7.19,0,11.26-4.31t4.09-11.72q0-7-4.05-11T366.8,17Z" style="fill:transparent;stroke:#fff;stroke-miterlimit:10;stroke-width:2" />
  </svg>
        </v-col>

      </v-row>

      <v-row>
        <v-spacer></v-spacer>
        <v-col>
          <h1 class="glitch">
            <span aria-hidden="true">Developer</span>
            Developer
            <span aria-hidden="true">Developer</span>
          </h1>
        </v-col>
      </v-row>

    </v-container>
  </section>
</template>

<style scoped>
.about-section {
  background: rgb(45, 51, 78);
  height: 100vh;
}
#supertitle {
  transform: translate(-50%, -50%);
  animation: fill 0.5s ease forwards 3.5s;
}
#supertitle path:nth-child(1) {
  stroke-dasharray: 187px;
  stroke-dashoffset: 187px;
  animation: line-anim 2s ease forwards;
}
#supertitle path:nth-child(2) {
  stroke-dasharray: 255px;
  stroke-dashoffset: 255px;
  animation: line-anim 2s ease forwards 0.3s;
}
#supertitle path:nth-child(3) {
  stroke-dasharray: 247px;
  stroke-dashoffset: 247px;
  animation: line-anim 2s ease forwards 0.6s;
}
#supertitle path:nth-child(4) {
  stroke-dasharray: 293px;
  stroke-dashoffset: 293px;
  animation: line-anim 2s ease forwards 0.9s;
}
#supertitle path:nth-child(5) {
  stroke-dasharray: 176px;
  stroke-dashoffset: 176px;
  animation: line-anim 2s ease forwards 1.2s;
}
#supertitle path:nth-child(6) {
  stroke-dasharray: 224px;
  stroke-dashoffset: 224px;
  animation: line-anim 2s ease forwards 1.5s;
}
#supertitle path:nth-child(7) {
  stroke-dasharray: 293px;
  stroke-dashoffset: 293px;
  animation: line-anim 2s ease forwards 1.8s;
}
#supertitle path:nth-child(8) {
  stroke-dasharray: 256px;
  stroke-dashoffset: 256px;
  animation: line-anim 2s ease forwards 2.1s;
}
@keyframes line-anim {
  to {
    stroke-dashoffset: 0;
  }
}
@keyframes fill {
  from {
    fill: transparent;
  }
  to {
    fill: white;
  }
}

.glitch {
  color: white;
  font-size: 6rem;
  font-weight: 700;
  text-transform: uppercase;
  position: relative;
  text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
    -0.025em -0.05em 0 rgba(0, 255, 0, 0.75),
    0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
  animation: glitch 500ms infinite;
}

.glitch span {
  position: absolute;
  top: 0;
  left: 0;
}

.glitch span:first-child {
  animation: glitch 650ms infinite;
  clip-path: polygon(0 0, 100% 0, 100% 45%, 0 45%);
  transform: translate(-0.025em, -0.0125em);
  /*   color: green; */
  opacity: 0.8;
}

.glitch span:last-child {
  animation: glitch 375ms infinite;
  clip-path: polygon(0 80%, 100% 20%, 100% 100%, 0 100%);
  transform: translate(0.0125em, 0.025em);
  /*   color: silver; */
  opacity: 0.8;
}
@keyframes glitch {
  0% {
    text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
      -0.05em -0.025em 0 rgba(0, 255, 0, 0.75),
      -0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
  }
  14% {
    text-shadow: 0.05em 0 0 rgba(255, 0, 0, 0.75),
      -0.05em -0.025em 0 rgba(0, 255, 0, 0.75),
      -0.025em 0.05em 0 rgba(0, 0, 255, 0.75);
  }
  15% {
    text-shadow: -0.05em -0.025em 0 rgba(255, 0, 0, 0.75),
      0.025em 0.025em 0 rgba(0, 255, 0, 0.75),
      -0.05em -0.05em 0 rgba(0, 0, 255, 0.75);
  }
  49% {
    text-shadow: -0.05em -0.025em 0 rgba(255, 0, 0, 0.75),
      0.025em 0.025em 0 rgba(0, 255, 0, 0.75),
      -0.05em -0.05em 0 rgba(0, 0, 255, 0.75);
  }
  50% {
    text-shadow: 0.025em 0.05em 0 rgba(255, 0, 0, 0.75),
      0.05em 0 0 rgba(0, 255, 0, 0.75), 0 -0.05em 0 rgba(0, 0, 255, 0.75);
  }
  99% {
    text-shadow: 0.025em 0.05em 0 rgba(255, 0, 0, 0.75),
      0.05em 0 0 rgba(0, 255, 0, 0.75), 0 -0.05em 0 rgba(0, 0, 255, 0.75);
  }
  100% {
    text-shadow: -0.025em 0 0 rgba(255, 0, 0, 0.75),
      -0.025em -0.025em 0 rgba(0, 255, 0, 0.75),
      -0.025em -0.05em 0 rgba(0, 0, 255, 0.75);
  }
}

@media (prefers-reduced-motion: reduce) {
  *,
  ::before,
  ::after {
    animation-delay: -1ms !important;
    animation-duration: 1ms !important;
    animation-iteration-count: 1 !important;
    background-attachment: initial !important;
    scroll-behavior: auto !important;
    transition-duration: 0s !important;
    transition-delay: 0s !important;
  }
}

</style>