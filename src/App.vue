<template>
  <!-- 외부 -->
  <div class="w-[56rem] h-[36rem]">
  <div class="flex max-w-screen-xl min-w-screen-sm min-h-full">
    <!-- 사이드 메뉴 -->
    <SideMenuComponent />
    <!-- 왼쪽 화면 (접히는 부분) -->
    <FriendsComponent />

    <!-- 오른쪽 화면 -->
    <MainComponent v-if="$store.state.modalStore.isMain"/>
    <ChatComponent v-if="$store.state.modalStore.isChat"/>
  </div>
  </div>

</template>

<script>
import SideMenuComponent from './components/SideMenuComponent.vue'
import FriendsComponent from './components/FriendsComponent.vue'
import MainComponent from './components/MainComponent.vue'
import ChatComponent from './components/ChatComponent.vue'

export default {
  name: 'App',
  components: {
    SideMenuComponent,
    FriendsComponent,
    MainComponent,
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
