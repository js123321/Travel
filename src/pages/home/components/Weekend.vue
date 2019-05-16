<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgURL" />
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgURL: 'http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg',
        title: '迪士尼乐园',
        desc: '全球最大的迪士尼乐园'
      }, {
        id: '0002',
        imgURL: 'http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg',
        title: '迪士尼乐园',
        desc: '全球最大的迪士尼乐园'
      }, {
        id: '0003',
        imgURL: 'http://img1.qunarzz.com/sight/source/1505/7d/df6ff468331c43.jpg_r_640x214_1f3783d0.jpg',
        title: '迪士尼乐园',
        desc: '全球最大的迪士尼乐园'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.recommend-title{
  margin-top :.2rem
  line-height .8rem
  background :#eee
  text-indent :.2rem
}
.item-img-wrapper{
  overflow :hidden
  height :0
  padding-bottom :33.9%
  .item-img{
    width :100%
  }
}
.item-info{
  padding :.1rem
  .item-title{
    line-height :.54rem
    font-size :.32rem
    ellipsis()
  }
  .item-desc{
    line-height :.4rem
    color :#ccc
    ellipsis()
  }
}
</style>
