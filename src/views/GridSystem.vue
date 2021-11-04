<template>

  <v-card>
    <v-card-title >
      Grid System
    </v-card-title>
    <v-card-text>

      <v-row>

        <v-col class="red" cols="12" sm="2" md="6" lg="10">A</v-col>
        <v-col class="green" cols="12" sm="10" md="6" lg="2">B</v-col>

      </v-row>

      <v-row class="indigo lighten-3">

        <v-col cols="12" sm="2" md="6" lg="10">A</v-col>
        <v-col cols="12" sm="10" md="6" lg="2">B</v-col>

      </v-row>
      
    </v-card-text>
  </v-card>

</template>
<script>
export default {
  // 컴포넌트의 대표이름(devtools에 나오는 이름)
  name: "",
  // 추가하고 싶은 컴포넌트 등록(import something from "/path")
  components: {},
  // 컴포넌트 데이터 정의
  data() {
    return {};
  },
  // 컴포넌트 메소드 정의
  methods: {},
};
</script>

<!-- 컴포넌트 스타일 정의 -->
<style scoped>
</style>