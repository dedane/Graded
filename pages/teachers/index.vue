<template>
  <v-content>
    <Drawer />
    <v-layout row-wrap>
      <Drawer />
      <v-flex xs12 md6>
        <v-card-media
          contain
          height="auto"
          src="https://ik.imagekit.io/ugyodiq15/Web_Development_da21db36-237c-42b4-9431-d57611436424_1024x1024_2x_acLC2MPL6.jpg"
        />
      </v-flex>
      <v-flex xs12 md6>
        <v-card-text>
          <v-form>
            <v-text-field
              id="id"
              name="name"
              outline
              label="name"
            />
            <v-text-field v-model="value" outline label="email" />
            <v-text-field v-model="value" outline label="Student Id" />
            <v-text-field v-model="value" required label="labWork" />
            <v-text-field v-model="value" required label="Quiz" />
            <v-text-field v-model="value" required label="MidSem" />
            <v-text-field v-model="value" required label="Finals" />
          </v-form>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn color="success">
            ADD
          </v-btn>
        </v-card-actions>
      </v-flex>
      <v-card-actions>
        <v-flex xs12 md6 align-start>
        <v-text-start-field />
        </v-flex>
      </v-card-actions>
    </v-layout>
    <Footer />
  </v-content>
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
