<template>
  <div class="min-w-20 w-20 bg-gradient-to-tl from-violet-400 to-indigo-600">
    <!-- 로고 -->

    <!-- 아이콘 리스트 -->
    <div class="w-full">
      <!-- 아이콘 컨테이너 -->
      <div class="mx-auto my-2 p-1 w-12 h-12" v-for="icon, index in icon_list" :key="index">
        <img class=" object-cover" :src="icon">
      </div>

    </div>
  </div>
</template>

<script>
export default {
  components: {

  },
  data(){
      return {
        icon_list: ['./assets/logo.png', './assets/emo-2.png', './assets/emo-3.png'],
      }
  },
  methods: {
    
  },
}
</script>

<style scoped>

</style>
