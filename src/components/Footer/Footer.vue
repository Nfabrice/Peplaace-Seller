<template>
    <div>
        <a-col class="container" :span="24">
            <a-col class="card" :span="3">
                <h5>Terms & Condition</h5>
            </a-col>
            <a-col class="card" :span="3">
                <h5>Cookie Policy</h5>
            </a-col>
            <a-col class="card" :span="3">
                <h5>Terms & Condition</h5>
            </a-col>
            <a-col class="card" :span="3">
                <h5>Terms & Condition</h5>
            </a-col>
            <a-col class="card" :span="3">
                <h5>Terms & Condition</h5>
            </a-col>
        </a-col>
        <a-col class="copyright" :span="24">
            ©️ 2010-2019 PePlaace.com. All rights reserved.
        </a-col>
    </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
    .container{
        display: flex;
    }.card{
        flex: 1;
        color: #665EFF;
        padding-top: 50px;
    } .card h5{
        color: #665EFF;
        justify-content: center;
    }
    .copyright{
        font-size: 12px;
        color: #665EFF;
    }
</style>
