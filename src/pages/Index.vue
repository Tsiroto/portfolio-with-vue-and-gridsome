<template>
  <Layout>
    <About />
    <Projects />
    <Warning />
    <Contact />
  </Layout>
</template>

<script>
import About from '@/components/About.vue'
import Projects from '@/components/Projects.vue'
import Warning from '@/components/Warning.vue'
import Contact from '@/components/Contact.vue'

export default {
  metaInfo: {
    title: 'Giorgos Ntoufas'
  },
  components: {
    About,
    Projects,
    Warning,
    Contact
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
