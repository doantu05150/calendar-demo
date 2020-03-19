<template>
  <div>
    <c-header :is-scroll="scrolled" />
    <div class="home-content">
      <el-main>
        <c-adaptive />
        <c-video />
        <c-work />
        <c-features />
      </el-main>
      <el-footer>
        <c-footer />
      </el-footer>
    </div>
  </div>
</template>

<script>
import { Header, Footer } from '@/components/common'
import {
  HomeAdaptive,
  HomeVideo,
  HomeWork,
  HomeFeatures
} from '@/components/home'

export default {
  layout: 'main',
  components: {
    'c-header': Header,
    'c-footer': Footer,
    'c-adaptive': HomeAdaptive,
    'c-video': HomeVideo,
    'c-work': HomeWork,
    'c-features': HomeFeatures
  },
  data() {
    return {
      scrolled: false
    }
  },
  mounted() {
    document.addEventListener('scroll', this.handleScroll)
  },
  beforeDestroy() {
    document.removeEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      this.scrolled = window.scrollY > 0
    }
  }
}
</script>

<style lang="scss" scoped>
.home-content {
  padding-top: 95px;
}
</style>
