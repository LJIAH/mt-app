<template>
  <div class="nav">
    <router-link class="nav-item" to="/goods">
      点菜
      <i class="line"></i>
    </router-link>
    <router-link class="nav-item" to="/ratings">
      评价
      <i class="line"></i>
    </router-link>
    <router-link class="nav-item" to="/seller">
      商家
      <i class="line"></i>
    </router-link> 
  </div>
</template>

<script>
export default {
  data () {
    return {
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav{
  display: flex;
  width: 100%;
  height: 40px;
  line-height: 40px;
  /* 下划线 */
  border-bottom: 1px solid #e4e4e4;
}
.nav-item{
  flex: auto;
  text-align: center;
  font-size: 13px;
  text-decoration: none;
  color: #666666;
  position: relative;
}

 /* 选中的样式 */
 .nav .active{
   color: #ffbb22;
 }

 /* 选中下面的下划线 */
 .nav .active .line{
   width: 20px;
   height: 2px;
   display: inline-block;
   background-color: #ffbb22;
   position: absolute;
   bottom: 0;
   left: 50%;
   margin-left: -10px;

 }

</style>
