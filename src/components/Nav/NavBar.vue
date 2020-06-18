<template>
  <div class="nav-bg">
    <div class="nav">
      <a><img @click="go" class="logo" alt="Peplace logo" src="../../assets/Logo.png"></a>
      <div class="avatar">
        <div class="username">
          <h5>John Doe</h5>
          <h6>@john_doe</h6>
        </div>
        <div class="profile">
          <img src="../../assets/avatarProfile.png" alt="">
        </div>
        <div class="menu">
          <button @click="go" class="home-menu"></button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  methods: {
    go () {
      this.$router.push('/')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*Navigation bar*/

.nav-bg{
  background-color: #E7F6FA;
  height: 379px;
  border-radius: 0 0 20px 20px;
}
.nav{
  position: absolute;
  display: flex;
  width: 100%;
  margin-top: 20px;
}
/* Brand */
.nav .logo{
  margin: 0 0 0 88px;
}

/* Avatar */
.nav .avatar{
  position: relative;
  display: flex;
  left: 74%;
}
.nav .avatar .username{
  position: relative;
  right: 20%;
}
.username h5{
  font-weight: bolder;
  color: black;
}
.username h6{
  color: #665EFF;
  margin-top: -7px;
  font-weight: bold;
}
/* Menu button */
button{
  border: none;
  border-radius: none;
  margin: 10px 10px 10px 20px;
}
.home-menu{
  background-image: url(../../assets/menu.png);
  width: 20px;
  height: 20px;
}
/* End - Navigation bar*/
</style>
