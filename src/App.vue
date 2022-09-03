<template>
  <div id="app">
    <router-view/>
    <h1>黑马头条</h1>
    <div>
      <i class="toutiao toutiao-dianzan2"></i>
      <van-button type="danger">危险按钮</van-button>
      <van-cell-group>
        <van-cell title="单元格" value="内容" />
        <van-cell title="单元格" value="内容" label="描述信息" />
      </van-cell-group>
      <van-icon name="chat-o" badge="9" />
      <van-cell is-link @click="showPopup">展示弹出层</van-cell>
      <van-popup v-model="show" closeable position="top" :style="{ height: '30%' }">内容</van-popup>
    </div>
  </div>
</template>
<script>
export default {
  name: 'App',
  data () {
    return {
      show: false
    }
  },

  methods: {
    showPopup () {
      this.show = true
    }
  }
}
</script>

<style lang="less">

</style>
