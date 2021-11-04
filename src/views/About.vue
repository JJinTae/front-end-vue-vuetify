<!-- 컴포넌트 UI 정의 -->
<template>
  <v-card class="mx-auto" width="300">
    <v-img src="@/assets/photos/photo1.jpg" height="250px" />
    <v-card-title >
      About
    </v-card-title>
    <v-card-subtitle>
      This is an about page
    </v-card-subtitle>
    <v-divider />
    <v-card-text>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos blanditiis itaque.
    </v-card-text>
    <v-divider />
    <v-card-text>
      dolores totam deleniti corporis fugit sequi quasi minima debitis dignissimos modi nisi qui recusandae dolore amet ipsa id vitae.
    </v-card-text>
    <v-card-actions>
      <div class="mx-auto">
      <v-btn class = "mr-2" color="success">OK</v-btn>
      <v-btn color="info">Cancel</v-btn>
      </div>
    </v-card-actions>
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