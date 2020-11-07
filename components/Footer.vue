<template>
  <div class="lighten-5 pa-10">
    <v-row no-gutters>
      <v-col cols="12" sm="6" md="8">
        <v-card class="pa-2" elevation="0"> <h2>TimeUp Logo</h2> </v-card>
      </v-col>
      <v-col cols="6" md="4">
        <v-card class="pa-2" elevation="0">
          Do not sell my info (California)
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" sm="6" md="8"
        ><v-card class="pa-2" elevation="0"> Visit Help Center</v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="5" sm="3" md="3"
        ><v-card class="pa-2" elevation="0">
          <h3>About us</h3>
          <v-list dense>Newsroom</v-list>
          <v-list dense>Investor relations</v-list>
          <v-list dense>Safety</v-list>
          <v-list dense>Blog</v-list>
          <v-list dense>ift cards</v-list>
        </v-card>
      </v-col>
      <v-col cols="12" sm="6" md="6">
        <v-card class="pa-2" elevation="0">
          <h3>More options</h3>
          <v-list dense>Order food</v-list>
          <v-list dense>Sign up to deliver</v-list>
          <v-list dense>View all cities</v-list>
          <v-list dense>FAQ</v-list>
          <v-list dense>Freight</v-list>
          <v-list dense>Health</v-list>
          <v-list dense>Elevate</v-list>
          <v-list dense>Advanced Technologies Group</v-list>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <div class="mr-16">F</div>
      <div class="mr-16">T</div>
      <div class="mr-16">Y</div>
      <div class="mr-16">L</div>
      <div class="mr-7">I</div>
      <div class="mr-10">English</div>
      <div class="mr-7">Yaounde</div>
    </v-row>
    <v-row>
      <v-footer :absolute="!fixed">
        <v-col cols="12" sm="6" md="6">
          <span
            >&copy; PaveWay Technologies Inc.
            {{ new Date().getFullYear() }}</span
          >
        </v-col>
        <v-col cols="12" sm="6" md="6">
          <p class="text-right">
            <span class="mr-16">Privacy</span>
            <span class="mr-16">Accessibility</span>
            <span class="mr-16">Terms</span>
          </p>
        </v-col>
      </v-footer>
    </v-row>
  </div>
</template>