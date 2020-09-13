<template>
  <Layout>
    <About />
    <Projects />
    <Timeline />
    <Contact />
  </Layout>
</template>

<script>
import About from '@/components/About.vue'
import Projects from '@/components/Projects.vue'
import Timeline from '@/components/Timeline.vue'
import Contact from '@/components/Contact.vue'

export default {
  metaInfo: {
    title: 'Giorgos Ntoufas'
  },
  components: {
    About,
    Projects,
    Timeline,
    Contact
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
</style>
