<template>
  <div class="header">
    <span class="header-txt">
      追书神器
    </span>
    <div class="header-sj">
      <router-link class="tubiao" to="/home" slot="right">
        <img src="./004.png">
      </router-link>
      <router-link class="tubiao" to="/search" slot="right">
        <img src="./003.png">
      </router-link>
      <router-link class="tubiao" to="/home" slot="right">
        <img src="./002.png">
      </router-link>
    </div>
      
    <!-- <router-link to="/mybooks">
    <ul class="header-sj" >
      <li><img src="./002.png"></li>
      <li class="search"><img src="./003.png"></li>
      <li class="fa"><img src="./004.png"></li>
      <i class="fa fa-book"></i>
      <span>书架</span>
    </ul>
    </router-link> -->
    <div class="header-tab">
      <router-link tag="a" class="tab-item" to="/mybooks">书架</router-link>
      <router-link tag="a" class="tab-item" to="/categories">分类</router-link>
      <router-link tag="a" class="tab-item" to="/rank">排行</router-link>
      <router-link tag="a" class="tab-item" to="/bookLists" >书单</router-link>
    </div>
  </div>
</template>
<script type="text/ecmascript-6">
  export default{

  }
</script>
<style scoped lang="stylus" rel="stylesheet/stylus">
  .header
    background-color tomato
    position relative
    .header-txt
      display inline-block
      font-size 35px
      color white
      font-weight 600
      padding 30px 15px
    .header-sj
      text-align center
      position absolute
      top 30px
      right 10px
      font-size 25px
      color #409EFF
      .tubiao
        width 15%
        float right 
        margin-right 10px;
      img 
        width 30%
        
        // vertical-align top
    .header-tab
      display flex
      .tab-item
        flex 1
        font-size 25px
        text-align center
        line-height 80px
        background tomato
        color #d6d6d6
      .router-link-active
        color #fff

</style>
