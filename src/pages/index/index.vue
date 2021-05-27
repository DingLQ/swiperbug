<template>
  <view class="index">
    <swiper
      indicatorColor='#999'
      indicatorActiveColor='#333'
      current="current"
      :duration="700"
      :circular="true"
      :autoplay="true"
      :indicatorDots="show">
      <swiper-item v-for="(item, idx) in imgUrls" :key="idx">
        <image :src="item" class="slide-image" />
      </swiper-item>
    </swiper>
  </view>
</template>

<script>
// 按需引入, 更小的应用体积
import './index.scss'
export default {
    components: {},
  data () {
    return {
      msg: 'Hello world!',
      imgUrls: [
        'https://img10.360buyimg.com/babel/s700x360_jfs/t25855/203/725883724/96703/5a598a0f/5b7a22e1Nfd6ba344.jpg!q90!cc_350x180',
        'https://img11.360buyimg.com/babel/s700x360_jfs/t1/4776/39/2280/143162/5b9642a5E83bcda10/d93064343eb12276.jpg!q90!cc_350x180',
        'https://img14.360buyimg.com/babel/s700x360_jfs/t1/4099/12/2578/101668/5b971b4bE65ae279d/89dd1764797acfd9.jpg!q90!cc_350x180',
      ],
      show: true,
    }
  },
  methods: {},
    }
</script>
