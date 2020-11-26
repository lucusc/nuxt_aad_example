<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <div class="text-center">
        <logo />
        <vuetify-logo />
      </div>
      <v-card>
        <v-card-title class="headline">
          Welcome to the Vuetify + Nuxt.js using Auth middleware
        </v-card-title>
        <v-card-text>
          <div v-if="!$auth.loggedIn">You need to log in.</div>
          <div v-else>You are logged in as {{ $auth.user.displayName }}</div>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo,
  },
  data() {
    return {
      message: '',
    }
  },
  methods: {
    testDebug() {
      this.message = 'Hello from a debugging'
    },
  },
}
</script>
