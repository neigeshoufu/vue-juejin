<template>
  <div :style="style" class="j-loading">
    
  </div>
</template>

<script>
  export default {
    props: {
      size: String
    },
    data() {
      return {
       style: {
         width: this.size,
         height: this.size,
         backgroundImage: `url(${require('./image/loading.gif')})`
       }
      }
    }
  }
</script>

<style lang="stylus" scoped>
.j-loading
  background-size cover
  background-repeat no-repeat
  background-position 50%
  border-radius 50%
</style>