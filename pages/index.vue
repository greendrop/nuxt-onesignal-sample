<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-xs-center" />
      <v-card>
        <v-card-title class="headline">
          Nuxt.js OneSignal Push通知サンプル
        </v-card-title>
        <v-card-text>
          <p>process.env</p>
          <ul>
            <li>ONESIGNAL_APP_ID: {{ onesignalAppId }}</li>
          </ul>
        </v-card-text>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  computed: {
    onesignalAppId() {
      return process.env.ONESIGNAL_APP_ID
    }
  }
}
</script>
