<template>
  <v-container grid-list-xs12 md6>
    <Drawer />
    <Results />
    <chart />
    <Footer />
  </v-container>
</template>

<script>
import Drawer from '../components/drawer'
import Results from '../components/results'
import Footer from '../components/footers'
import chart from '../components/chart'

export default {
  head() {
    return {
      title: 'HOME'
    }
  },
  components: {
    Drawer,
    Results,
    chart,
    Footer
  }
}
</script>
<style>

</style>
