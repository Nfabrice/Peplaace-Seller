<template>
    <div class="create-store">
        <div class="store">
            <a-row>
                <div class="menu">
                    <a-menu
                    class="menu-bar"
                    :default-selected-keys="['1']"
                    :default-open-keys="['sub1']"
                    mode="inline"
                    theme="dark"
                    :inline-collapsed="collapsed">
                    <!-- 1st menu option -->
                    <a-page-header
                        class="title"
                        style="solid rgb(235, 237, 240);"
                        @back="() => null">
                        <a-icon type="arrow-left" /> Create Store
                    </a-page-header>
                        <!-- Menu Items -->
                        <a-menu-item class="item" style="height: 100px;" key="1">
                            <div class="item-description">
                                <a-icon type="left-circle" />
                                <span>Primary Info</span> <br>
                                <p>Name, About your store, how you work, Connected PePlaace account.</p>
                            </div>
                        </a-menu-item>
                        <!-- 2nd menu option -->
                        <a-menu-item style="height: 100px;" key="2">
                            <a-icon type="left-circle" />
                            <span>Locations</span> <br>
                            <p>Main location for your business as a store.</p>
                        </a-menu-item>
                        <!-- 3rd menu option -->
                        <a-menu-item style="height: 100px;" key="3">
                            <a-icon type="left-circle" />
                            <span>Currency and Billing</span>
                            <p>Which currency do you prefer? Payment Credentials Deposit and Credit, e.t.c</p>
                        </a-menu-item>
                        <!-- 4th menu option -->
                        <a-menu-item style="height: 100px;" key="4">
                            <a-icon type="left-circle" />
                            <span>Terms that Apply</span>
                            <p>Tick and finish, continue to furnish your sales!!</p>
                        </a-menu-item>
                        <!-- 5th menu option -->
                        <a-menu-item style="height: 100px;">
                        </a-menu-item>
                        <!-- 5th menu option -->
                        <a-menu-item style="height: 100px;" key="5">
                            <button class="side-menu-btn-a btn"><a-icon type="arrow-left" />Previous</button>
                            <button @click="next" class="side-menu-btn-b btn"><a-icon type="arrow-right" />Next</button>
                        </a-menu-item>
                    </a-menu>
                </div>
            </a-row>
        </div>
            <storeHome/>
    </div>
</template>
<script>
import StoreHome from '@/components/CreateStoreMenu/StoreHome.vue'
export default {
  name: 'Menu',
  components: {
    StoreHome
  },
  data () {
    return {
      collapsed: false
    }
  },
  methods: {
    toggleCollapsed () {
      this.collapsed = !this.collapsed
    },
    next () {
      this.$router.push('/CreateStoreHome')
    }
  }
}
</script>

<style scoped>

.boxes{
    border-radius:  10px 10px 0 0;
    margin: -260px 0 0 0;
}
.create-store{
        align-content: center;
        background-color: white;
        display: flex;
        height: 100%;
        border-radius:  10px 10px 0 0;
        margin: -250px 200px 0 200px;
        box-shadow:
            0 0px 2.2px rgba(0, 0, 0, 0.017),
            0 0px 5.3px rgba(0, 0, 0, 0.024),
            0 0px 10px rgba(0, 0, 0, 0.03),
            0 0px 17.9px rgba(0, 0, 0, 0.036),
            0 0px 33.4px rgba(0, 0, 0, 0.043),
            0 0px 80px rgba(0, 0, 0, 0.06);
}

.menu{
    width: 75%;
    border-style: solid;
    border-radius: 1%;
    border-color: rgb(0, 0, 32);
}
.menu-bar{
    text-align: left;
}
.btn{
    width: 98px;
    background-color: #f4fcfd0c;
    border-color: transparent;
    border-radius: 4px;
}
.side-menu-btn-a{
    margin-right: 73px;
}
.side-menu-btn-b{
    margin-left: 69px;
}.item-description{
    font-size: 12px
}.title{
    color:white;
}.create-store-text{
    width: 100%;
    text-align: center;
}.create-store-text h1{
    color: #0B1237;
    font-weight: bolder;
}
</style>
