<template>
    <div>
        <NavBar/>
        <Menu />
    </div>
</template>
<script>
import NavBar from '@/components/Nav/NavBar.vue'
import Menu from '@/components/CreateStoreMenu/Menu.vue'
export default {
  name: 'CreateStoreHome',
  components: {
    NavBar,
    Menu
  }
}
</script>
<style lang="less" scoped>

</style>
