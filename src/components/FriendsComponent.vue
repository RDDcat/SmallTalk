<template>
  <div class="inline-block w-5/12 h-full">    
    <!-- 타이틀 -->
    <div class="ml-4 my-4 font-semibold text-2xl">
      친구
    </div>
    <!-- 친구 목록 -->
    <div class="flex flex-col max-h-screen overflow-hidden overflow-y-auto">
      <!-- 친구 컴포넌트 -->
      <div 
        class="flex w-full h-16 px-4 my-1" v-for="friend, index in friends" :key="index"
        :class="select===index?'bg-gray-200':''"
        >
        <!-- 이미지 -->
        <div class="my-auto h-5/6 rounded-full">
          <img class="w-full h-full object-cover" src="@/assets/profile.png">
        </div>
        <!-- 사용자 정보 -->
        <div class="flex flex-col w-auto h-full py-1">
          <!-- 사용자 명 -->
          <div class="font-semibold text-base pl-2 my-auto">
            {{friend.user_name}}
          </div>
          <!-- 최근 메시지 -->
          <div class="text-sm w-9/12 pl-2 my-auto text-gray-400 truncate">
            {{ friend.latest_message }}
          </div>
        </div>
        <!-- 시간과 메시지 알림 -->
        <div class="flex flex-col w-auto h-full py-1 ml-auto mr-4">
          <!-- 시간 -->
          <div class="font-semibold text-base pl-2 my-auto text-gray-400">
            {{ friend.date }}
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
        friends:[
          {user_name:'김성준', latest_message: '뭐하누~!!!!!!!!!!', date:'5.11'},
          {user_name:'D', latest_message: 'Slay~~~', date:'5.11'},
          {user_name:'Gumi', latest_message: '구미베어~ ', date:'5.11'},

        ],
        select:0,
      }
  },
  methods: {
    
  },
}
</script>

<style scoped>

</style>
