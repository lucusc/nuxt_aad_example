<template>
  <div v-if="!$auth.loggedIn">
    <v-btn @click="$auth.loginWith('aad')">Sign In </v-btn>
  </div>
  <div v-else>
    {{ $auth.user.displayName }}
    <v-btn icon fab small @click="$auth.logout('aad')">
      <v-icon>mdi-logout</v-icon>
    </v-btn>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
