<template>
  <div class="new-store">
    <NavBar/>
    <Menu/>
  </div>
</template>
<script>
import NavBar from '@/components/Nav/NavBar.vue'
import Menu from '@/components/CreateStoreMenu/Menu.vue'
export default {
  name: 'CreateStore',
  components: {
    NavBar,
    Menu
  }
}
</script>
<style lang="less" scoped>

</style>
