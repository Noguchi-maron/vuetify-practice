<template>
<v-app>
  <v-navigation-drawer app mx-auto my-0>
    <v-btn text block>TopPage</v-btn><br>
    <v-btn text block>About</v-btn>
  </v-navigation-drawer>

  <v-app-bar app>
    TodoList
  </v-app-bar>

  <!-- Sizes your content based upon application components -->
  <v-main>

    <!-- Provides the application the proper gutter -->
    <v-container fluid>
      <v-form>
      <v-col md="4" sm="6">
      <v-text-field v-model="msg" label="FirstName" clearable>
      </v-text-field>
      </v-col>
      <v-col md="4" sm="6">
      <v-text-field v-model="msg" label="LastName" clearable>
      </v-text-field>
      </v-col>
      <v-btn elevation="0" outlined class="font-weight-bold">
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
