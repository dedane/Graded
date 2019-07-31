<template>
  <div>
    <v-layout-wrap>
      <Drawer />
      <Footer />
    </v-layout-wrap>
  </div>
</template>
<style>
</style>
<script>
import Drawer from '../../components/drawer'
import Footer from '../../components/footers'
export default {
  head() {
    return {
      title: 'HOME'
    }
  },
  components: {
    Drawer,
    Footer
  }
}
</script>
