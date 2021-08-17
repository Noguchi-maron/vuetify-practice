<template>
<v-app>
  <v-navigation-drawer app>
    <a>TopPage</a><br>
    <a>About</a>
  </v-navigation-drawer>

  <v-app-bar app>
    TodoList
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>
      <v-form>
      <v-col sm="6">
      <v-text-field v-model="msg" label="Name" clearable @focus="isFocus=true" @blur="isFocus=false">
      </v-text-field>
      </v-col>
      <v-btn elevation="2">
        送信
      </v-btn>

      </v-form>
      <!-- If using vue-router -->
    </v-container>
  </v-main>

  <v-footer app>
    <!-- -->
  </v-footer>
</v-app>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {
      msg: '',
      isFocus: false
    }
  },
  components: {
  },
}
</script>
