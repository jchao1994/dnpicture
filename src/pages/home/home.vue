<template>
  <view class="home">
    <tabs :items="tabsItems"></tabs>
    <home-recommend></home-recommend>
    <home-category></home-category>
    <home-new></home-new>
    <home-album></home-album>
  </view>
</template>

<script>
  import homeRecommend from './childComps/home-recommend/homeRecommend';
  import homeCategory from './childComps/home-category/homeCategory';
  import homeNew from './childComps/home-new/homeNew';
  import homeAlbum from './childComps/home-album/homeAlbum';

  import tabs from '@/components/tabs/tabs';

export default {
  data() {
    return {
      tabsItems: ['选项卡1','选项卡2','选项卡3']
    }
  },
  components: {
    homeRecommend,
    homeCategory,
    homeNew,
    homeAlbum,
    tabs
  }
}
</script>

<style>

</style>