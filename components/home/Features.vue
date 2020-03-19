<template>
  <div>
    <section>
      <div class="sub-section">
        <div class="container">
          <el-container>
            <div class="w-full">
              <div class="font-bold h-title wide w-full">
                Features that everyone will enjoy
              </div>
              <div class="w-full mt-4 mb-10">
                <img
                  src="https://assets.calendly.com/assets/landing/en/homepage/features-3648204d046c9441528ae85ac7d5a01b9240d013cfabd0af34026671cb8322da.png"
                  class="img-fluid"
                  alt="img"
                />
              </div>
              <el-row class="mb-10">
                <el-col
                  v-for="item in 3"
                  :key="`p1_${item}`"
                  :style="getPaddingItem(item)"
                  :span="8"
                >
                  <div class="h-title font-bold">
                    <i class="el-icon-date mr-2" />
                    Calendar Integrations
                  </div>
                  <p class="hp">
                    Works with your Google, Outlook, Office 365 or iCloud
                    calendar so you’re never double booked
                  </p>
                </el-col>
              </el-row>
              <el-row class="mb-10">
                <el-col
                  v-for="item in 3"
                  :key="`p1_${item}`"
                  :style="getPaddingItem(item)"
                  :span="8"
                >
                  <div class="h-title font-bold">
                    <i class="el-icon-date mr-2" />
                    Calendar Integrations
                  </div>
                  <p class="hp">
                    Works with your Google, Outlook, Office 365 or iCloud
                    calendar so you’re never double booked
                  </p>
                </el-col>
              </el-row>
              <div class="text-center">
                <a href="#" class="more-features">Learn more about features</a>
              </div>
            </div>
          </el-container>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  methods: {
    getPaddingItem(index) {
      switch (index) {
        case 1:
          return { paddingRight: '40px' }
        case 2:
          return { padding: '0 20px' }
        case 3:
          return { paddingLeft: '40px' }
        default:
          break
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.wide {
  padding-bottom: 20px;
  font-size: 30px;
  text-align: center;
}

.mt-4 {
  margin-top: 16px;
}

.mb-10 {
  margin-bottom: 40px;
}

.mr-2 {
  margin-right: 8px;
}

.more-features {
  color: var(--main-color);
  text-decoration: none;
}
</style>
