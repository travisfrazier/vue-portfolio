<template>
  <Layout>
    <About />
    <Projects />
    <Contact />
  </Layout>
</template>

<script>
import About from '~/components/About.vue'
import Projects from '~/components/Projects.vue'
import Contact from '~/components/Contact.vue'

export default {
  metaInfo: {
    title: 'Hello, world!'
  },
  components: {
    About,
    Projects,
    Contact
  }
}
</script>

<style>

</style>
