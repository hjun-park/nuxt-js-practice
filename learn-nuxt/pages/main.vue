<template>
  <div>
    <p>메인 페이지입니다</p>
  </div>
</template>

<script>
// axios 이슈 [조치방법: https://www.inflearn.com/questions/672613]
import axios from 'axios';

export default {
  // created를 통해서 products Main을 그림
  // 이렇게 되면 노드서버 (/backend) 내의 products 데이터들을 들고옴
  async created() {
    const response = await axios.get('http://localhost:3000/products')
    console.log(response)
  }
}
</script>

<style lang="scss" scoped>

</style>