<template>
    <div class="store">
    <a-row>
        <a-col class="card" :span="24">
            <a-col class="art">
                <img src="../../assets/art.png" alt="">
            </a-col>
            <a-col class="create-store" :span="24" :offset="8">
                <a-row class="store" :span="12">
                    <a-col :span="6">
                        <img class="store-logo" src="../../assets/Nike.png" alt="">
                    </a-col>
                    <a-col class="store-details" :span="6">
                        <h4>Nike Store - Rwanda</h4>
                        <h5>Rwanda<a href="">(Pro)</a></h5>
                    </a-col>
                </a-row>
                <a-row class="store" :span="12">
                    <a-col  :span="6">
                        <img class="store-logo" src="../../assets/Chanel.png" alt="">
                    </a-col>
                    <a-col class="store-details" :span="6">
                        <h4>Nike Store - Rwanda</h4>
                        <h5>Rwanda<a href="">(Pro)</a></h5>
                    </a-col>
                </a-row>
                <a-row class="store" :span="12">
                    <a-col :span="6">
                        <img class="store-logo" src="../../assets/Boss.png" alt="">
                    </a-col>
                    <a-col class="store-details" :span="6">
                        <h4>Nike Store - Rwanda</h4>
                        <h5>Rwanda<a href="">(Pro)</a></h5>
                    </a-col>
                </a-row>
                <a-row class="create-store-btn" :span="12">
                    <button @click="create" class="btn"> <img src="../../assets/store.png" alt=""> CREATE STORE</button>
                </a-row>
            </a-col>
        </a-col>
        <a-col :span="24">
            <a-col class="mid-logo" :span="24">
                <img src="../../assets/Logo.png" alt="Peplace Logo">
            </a-col>
        </a-col>
    </a-row>
    </div>
</template>

<script>
export default {
  name: 'Body',
  methods: {
    create () {
      this.$router.push('/createStore')
    }
  }
}
</script>

<style scoped>
    .art{
        margin: -300px 0 0 160px;
    }
    .create-store{
        align-content: center;
        background-color: white;
        height: 450px;
        width: 558px;
        border-radius:  15px 15px 0 0;
        margin-top: -350px;
        border-top-style: solid;
        border-color: #665EFF;
        box-shadow:
            0 0px 2.2px rgba(0, 0, 0, 0.017),
            0 0px 5.3px rgba(0, 0, 0, 0.024),
            0 0px 10px rgba(0, 0, 0, 0.03),
            0 0px 17.9px rgba(0, 0, 0, 0.036),
            0 0px 33.4px rgba(0, 0, 0, 0.043),
            0 0px 80px rgba(0, 0, 0, 0.06)
;

;
    } .create-store-btn{
        height: 67px;
    }
    .btn{
        color: #665EFF;
        font-size: 12px;
        font-weight: bolder;
        border: none;
        margin: 23.5px 10px 10px 10px;
        text-decoration: none;
        cursor: context-menu;
        background-color: transparent;
    }
    .store-logo{
        width: 80px;
        margin: 30px 0 0 0;
    }
    .store-details{
        margin: 40px 20px 20px 0;
    }
    .store-details h4{
        font-size: 16px;
        font-weight: bolder;
        color: black;
        width: 200px;
    }
    .store-details h5 {
        font-size: 14px;
        font-weight: normal;
        color: #78849E;
    }.mid-logo{
        padding: 60px;
    }
    button{
        text-decoration: none;
    }
    button:focus {
        outline: none;
    }
</style>
