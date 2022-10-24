<template>
  <!-- 레이아웃 -> 페이지 -> 공통 컴포넌트 렌더링 된다고 보면 됨 -->
  <!-- $route 객체 이름 전달-->
  <div>
    <h1>{{ $route.name }} 페이지</h1>
    <Nuxt />
  </div>

  
</template>

<script>
export default {
  created() {
    console.log(this.$route)
  },
}
</script>
