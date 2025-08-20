<template>
  <view class="index">
    <nut-cell title="路由参数" :desc="instance.router.params.id"></nut-cell>
    <nut-button @click="onTryRequest">发起请求</nut-button>
    <span :class="$style.greenText">这是cssModule测试</span>
  </view>
</template>

<script setup>
import Taro from '@tarojs/taro'

const instance = Taro.getCurrentInstance()
definePageConfig({
  navigationBarTitleText: 'PageB',
})

function onTryRequest() {
  // TODO
}
</script>

<style lang="scss" module>
.greenText {
  color: var(--color-success);
}
</style>
