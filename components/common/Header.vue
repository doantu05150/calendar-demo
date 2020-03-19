<template>
  <div class="navbar" :class="isScroll && 'shadow'">
    <div class="header-wrapper">
      <div class="header">
        <a href="#" class="logo">
          <img
            src="https://assets.calendly.com/assets/landing/logo-322b42cc2dbb65ee44833c643677cbcd7e8a35bc4c15ae429715d2dec882fc57.png"
            alt="logo"
          />
        </a>
        <el-menu
          :default-active="activeIndex"
          class="el-menu-demo"
          mode="horizontal"
          text-color="#cecece"
          active-text-color="#ffd04b"
        >
          <el-menu-item
            v-for="(item, index) in navItems"
            :key="`nav_${index}`"
            :index="`${index + 1}`"
            class="nav-item"
            >{{ item.title }}</el-menu-item
          >
          <el-menu-item index="98" class="nav-item nav-btn"
            ><span class="btn">Sign up</span></el-menu-item
          >
          <el-menu-item index="99" class="nav-item nav-btn"
            >Sign in</el-menu-item
          >
        </el-menu>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    isScroll: {
      type: Boolean,
      required: true
    }
  },
  data() {
    return {
      activeIndex: '4',
      navItems: [
        {
          title: 'Features',
          href: '#'
        },
        {
          title: 'Pricing',
          href: '#'
        },
        {
          title: 'Integrations',
          href: '#'
        },
        {
          title: 'Solutions',
          href: '#'
        },
        {
          title: 'For Teams',
          href: '#'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.navbar {
  position: fixed;
  width: 100%;
  top: 0;
  left: 0;
  background-color: #fff;
  z-index: 99;

  .header-wrapper {
    padding: 0 20px;
    max-width: var(--main-width);
    margin: 0 auto;

    .header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px 0;

      img {
        width: 115px;
        height: 35px;
      }

      .nav-item {
        color: #666a73 !important;
        font-size: 14px;
        letter-spacing: 1px;
        padding: 0 13px;
        background-color: transparent;

        ::hover {
          text-decoration: underline !important;
        }
      }

      .btn {
        padding: 6px 10px;
        background-color: var(--main-color);
        color: #fff;
        border-radius: 4px;

        ::hover {
          background-color: var(--main-color-lighten);
        }
      }
    }
  }
}
.shadow {
  box-shadow: 0 7px 20px -5px rgba(0, 0, 0, 0.2);
}
// custom
.is-active {
  border-bottom-color: transparent !important;
}
.el-menu.el-menu--horizontal {
  border-bottom: none !important;
}
</style>
