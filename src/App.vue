<template>
  <!-- 외부 -->
  <div class="w-[40rem] h-96">
  <div class="flex max-w-screen-xl min-w-screen-sm min-h-full">
    <!-- 사이드 메뉴 -->
    <SideMenuComponent />
    <!-- 왼쪽 화면 (접히는 부분) -->
    <FriendsComponent />

    <!-- 오른쪽 화면 -->
    <ChatComponent />
  </div>
  </div>

</template>

<script>
import SideMenuComponent from './components/SideMenuComponent.vue'
import FriendsComponent from './components/FriendsComponent.vue'
import ChatComponent from './components/ChatComponent.vue'

export default {
  name: 'App',
  components: {
    SideMenuComponent,
    FriendsComponent,
    ChatComponent,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
