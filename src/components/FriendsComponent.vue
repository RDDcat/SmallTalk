<template>
  <div class="inline-block h-full">    
    <!-- 타이틀 -->
    <div class="ml-4 my-4 font-semibold text-2xl">
      친구
    </div>
    <!-- 친구 목록 -->
    <div class="flex flex-col w-96 overflow-x-hidden overflow-y-auto">
      <!-- 친구 컴포넌트 -->
      <div class="flex w-full h-14 px-4 my-3">
        <!-- 이미지 -->
        <div class="my-auto w-12 h-12 rounded-full">
          <img class="w-full h-full object-cover" src="@/assets/profile.png">
        </div>
        <!-- 사용자 정보 -->
        <div class="flex flex-col w-auto h-full py-1">
          <!-- 사용자 명 -->
          <div class="font-semibold text-base pl-2 my-auto">
            김성준
          </div>
          <!-- 최근 메시지 -->
          <div class="text-sm pl-2 my-auto">
            뭐하누~!!!!!!!!!!
          </div>
        </div>
        <!-- 시간과 메시지 알림 -->
        <div class="flex flex-col w-auto h-full py-1 ml-auto mr-4">
          <!-- 시간 -->
          <div class="font-semibold text-base pl-2 my-auto">
            5.11
          </div>
          <!-- 알림 -->
          <div class="text-sm pl-2 my-auto mx-auto">
            !
          </div>
        </div>
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

      }
  },
  methods: {
    
  },
}
</script>

<style scoped>

</style>
