<template>
  <div class="hm-stories-card">
    <div class="primary">
      <div class="title">
        <text class="text">{{ options.text }}</text>
        <image class="titleImg" :src="options.titleImg" />
      </div>
      <div class="block">
        <div class="outer">
          <div class="tianjiaWrap">
            <image class="tianjia" :src="options.tianjia" />
          </div>
        </div>
        <div class="color" />
        <div class="avatorWrap">
          <image class="avator" :src="options.avator" />
        </div>
        <div class="group">
          <image class="largeIcon" :src="options.largeIcon" />
        </div>
        <div class="container"><image class="img" :src="options.img" /></div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmStoriesCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-stories-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          text: '故事与瞬间',
          titleImg:
            '/static/hm-stories-card/images/img_24025_0_0.png',
          tianjia:
            '/static/hm-stories-card/images/img_24025_0_4.png',
          avator:
            '/static/hm-stories-card/images/img_24025_0_1.png',
          largeIcon:
            '/static/hm-stories-card/images/img_24025_0_3.png',
          img:
            '/static/hm-stories-card/images/img_24025_0_2.png'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
