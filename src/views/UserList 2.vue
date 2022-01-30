<template>
  <v-app id="inspire">

    <h2>ユーザー一覧</h2>

    <v-main>
      <v-container>
        <v-row>
          <v-col
            v-for="n in 24"
            :key="n"
            cols="4"
          >
          <router-link :to="{ path: '/chat', query: { user_id: n }}">
            <v-avatar color="grey lighten-2" size="128"></v-avatar>
          </router-link>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
  export default {
    //
  }
</script>