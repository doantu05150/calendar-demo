<template>
  <div>
    <c-header :is-scroll="scrolled" />
    <div class="content">
      <client-only>
        <v-date-picker
          mode="range"
          :value="null"
          title-position="left"
          color="teal"
          is-inline
        />
      </client-only>
      <el-calendar :value="null" />
    </div>
  </div>
</template>

<script>
import Header from '@/components/common/Header'

export default {
  components: {
    'c-header': Header
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
.content {
  padding-top: 95px;
}
</style>
