<template>
  <v-app>
    <v-row
    align="center"
    justify="space-around"
  >
    <v-btn depressed>
      Normal
    </v-btn>
    <v-btn
      depressed
      color="primary"
    >
      Primary
    </v-btn>
    <v-btn
      depressed
      color="error"
    >
      Error
    </v-btn>
    <v-btn
      depressed
      disabled
    >
      Disabled
    </v-btn>
  </v-row>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
