<!-- 컴포넌트 UI 정의 -->
<template>
  <v-app>

    <v-navigation-drawer app dark v-model="drawer">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title class="text-h6">
            Application
          </v-list-item-title>
          <v-list-item-subtitle>
            with Vue + Vuetify
          </v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list dense nav>
        <v-list-item to="/">
        <v-list-item-icon>
          <v-icon>mdi-home</v-icon>
        </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item to="/about">
          <v-list-item-icon>
            <v-icon>mdi-help-circle</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>About</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-group :value="false" prepend-icon="mdi-palette-outline" active-class="yellow--text">
          <template v-slot:activator>
            <v-list-item-title>Styles</v-list-item-title>
          </template>

          <v-list-item to="/styles/textandtypography" color="white">
            <v-list-item-icon></v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Text and Typography</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

          <v-list-item to="/styles/spacing" color="white">
            <v-list-item-icon></v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Margin and Padding</v-list-item-title>
            </v-list-item-content>
          </v-list-item>

        </v-list-group>

        <v-list-item to="/gridsystem">
          <v-list-item-icon>
            <v-icon>mdi-view-grid-outline</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Gird System</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        
      </v-list>

    </v-navigation-drawer>

    <v-main>

      <v-app-bar app color="secondary" dark>
        <v-app-bar-nav-icon @click="drawer=!drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Collapsing Bar</v-toolbar-title>
      </v-app-bar>


      <v-container fluid>
        <router-view></router-view>
      </v-container>

    </v-main>

    <v-footer app color="secondary" dark>
      <div class="mx-auto">K.J.T</div>
    </v-footer>

  </v-app>
</template>

<script>
export default {
  // 컴포넌트의 대표이름(devtools에 나오는 이름)
  name: "App",
  // 추가하고 싶은 컴포넌트 등록(import something from "/path")
  components: {},
  // 컴포넌트 데이터 정의
  data() {
    return {
      drawer: false,

    };
  },
  // 컴포넌트 메소드 정의
  methods: {},
  props: [

  ]
};
</script>

<!-- 컴포넌트 스타일 정의 -->
<style scoped>
</style>