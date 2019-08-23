<template>
  <v-app>
    <v-app-bar dark app>
      <v-toolbar-title class="mr-2"><img src="./assets/coc_logo.png" height="50"></v-toolbar-title>
      <v-toolbar-title class="headline text-uppercase">
        <span>COC&nbsp;</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text dark>Competitive</v-btn>
      
    </v-app-bar>

    <v-content>
      <v-container fluid fill-height justify-center class="pa-0"><router-view /></v-container>
    </v-content>

    <PageFooter />
  </v-app>
</template>

<script>
import PageFooter from '@/components/PageFooter'
export default {
  name: 'App',
  components: {
    PageFooter
  },
  data: () => ({
    //
  }),
};
</script>
