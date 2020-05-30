<template>
  <view class="tabs">
    tabs
    <uni-segmented-control :current="current" :values="items" @clickItem="onClickItem"></uni-segmented-control>
  </view>
</template>

<script>
import {uniSegmentedControl} from "@dcloudio/uni-ui"

export default {
  data() {
    return {
      current: 0
    }
  },
  props: {
    items: {
      type: Array,
      default() {
        return [];
      }
    }
  },
  methods: {
    onClickItem(e) {
      if (this.current !== e.currentIndex) {
        this.current = e.currentIndex;
      }
    }
  },
  components: {
    uniSegmentedControl
  }
}
</script>

<style>
</style>