<template>
<v-app>
  <v-navigation-drawer app mx-auto my-0>
    <v-btn text>TopPage</v-btn><br>
    <v-btn text>About</v-btn>
  </v-navigation-drawer>

  <v-app-bar app>
    TodoList
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>
      <v-form>
      <v-col sm6>
      <v-text-field v-model="msg" label="Name" clearable>
      </v-text-field>
      </v-col>
      <v-btn elevation="2" outlined class="font-weight-bold">
        保存
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
    }
  },
  components: {
  },
}
</script>
