<template>
  <v-content-wrap xs12 md6>
    <v-card flat class="result">
      <v-toolbar flat>
        <v-toolbar-title class="grey--text">
          Results
        </v-toolbar-title>
        <v-spacer width="10" />
        <v-btn icon>
          <v-icon>search</v-icon>
        </v-btn>
      </v-toolbar>

      <v-row>
        <v-container fluid grid-list-xs>
          <v-layout wrap>
            <v-flex v-for="i in 1" :key="i">
              <v-card width="400" height="100">
                <v-subheader>John Ogutu</v-subheader>
                <v-avatar>
                  <v-img src="https://ik.imagekit.io/ugyodiq15/id6_4zq-EdZQcJ.jpg" />
                </v-avatar>
              </v-card>
              <v-spacer />
              <v-card width="400" height="100">
                <v-subheader>Martha Ndungu</v-subheader>
                <v-avatar>
                  <v-img src="https://ik.imagekit.io/ugyodiq15/id2_Nls02YKVS.jpg" />
                </v-avatar>
              </v-card>
            </v-flex>
          </v-layout>
          <v-spacer />
        </v-container>
        <v-container fluid grid-list-xs>
          <v-layout wrap>
            <v-flex v-for="i in 1" :key="i">
              <v-card width="400" height="100">
                <v-subheader>Sharlene Muriki</v-subheader>
                <v-avatar>
                  <v-img src="https://ik.imagekit.io/ugyodiq15/id4_3MBxZA2Xm.jpg" />
                </v-avatar>
              </v-card>
              <v-card width="400" height="100">
                <v-subheader>Amina Sarai</v-subheader>
                <v-avatar>
                  <v-img src="https://ik.imagekit.io/ugyodiq15/id1_u9f8VIxRK.jpg" />
                </v-avatar>
              </v-card>
            </v-flex>
          </v-layout>
          <v-spacer />
        </v-container>
      </v-row>
    </v-card>
  </v-content-wrap>
</template>
<style>
</style>
<script>
export default {
  head() {
    return {
      title: 'Home'
    }
  }
}
</script>
