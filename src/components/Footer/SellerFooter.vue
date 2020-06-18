<template>
    <a-row class="container" :span="24">
        <a-row type="flex" justify="space-around" align="middle">
      <a-col :span="2">
        <div class="center">
            <h4>BUSINESS</h4>
            <h5 v-for="(data) in business" :key="data">{{data.key}}</h5>
        </div>
      </a-col>
      <a-col :span="2">
        <div class="center">
          <h4>PERSONAL</h4>
          <h5 v-for="(data) in personal" :key="data">{{data.key}}</h5>
        </div>
      </a-col>
      <a-col :span="2">
        <div class="center">
          <h4>DEVELOPERS</h4>
          <h5 v-for="(data) in developers" :key="data">{{data.key}}</h5>
        </div>
      </a-col>
      <a-col class="ftr-links" :span="2">
        <div class="center">
            <h4>HELP & SUPPORT</h4>
          <h5 v-for="(data) in support" :key="data">{{data.key}}</h5>
        </div>
      </a-col>
    </a-row>
    </a-row>
</template>
<script>
export default {
  name: 'SellerFooter',
  data () {
    return {
      business: [
        { key: 'Open Store', link: 'https://www.antdv.com/components/auto-complete/#Customized' },
        { key: 'Customers', link: '' },
        { key: 'Collection', link: '' },
        { key: 'Product Categories', link: '' },
        { key: 'Claim IP' }
      ],
      personal: [
        { key: 'Account Settings', link: '' },
        { key: 'Setup Profile', link: '' },
        { key: 'Currency', link: '' },
        { key: 'Report' }
      ],
      developers: [
        { key: 'API', link: '' },
        { key: 'Statistics', link: '' },
        { key: 'Report Bug', link: '' },
        { key: 'Beta Versions', link: '' },
        { key: 'Claim IP' }
      ],
      support: [
        { key: 'Orders', link: '' },
        { key: 'Shipping', link: '' },
        { key: 'Help Portal', link: '' },
        { key: 'Customer Services', link: '' }
      ]
    }
  }
}
</script>
<style scoped>
    .container{
        height: 100%;
        color: #665EFF;
    } .height-100{
        margin-top: 40px;
        display: block;
        background-color: rgb(191, 252, 252);
        width: 150px;
    } .center h4{
        color: #665EFF;
        font-size: 12px;
        font-weight: bolder;
    }
    .height-100 h5{
        color: #2A2E43;
        font-size: 14px;
        font-weight: normal;
    } .ftr-links .height-100{
        justify-content: left;
    }.center{
      text-align: left;
      height: 100%;
      margin: 0;
      padding: 0;
    }
</style>
