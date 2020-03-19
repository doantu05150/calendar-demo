<template>
  <div>
    <section>
      <div class="sub-section">
        <div class="container">
          <el-container>
            <div class="w-full">
              <div class="h-title wide w-full text-center">
                Get started for free today
              </div>
              <el-row justify="middle">
                <el-col :span="12" :offset="6">
                  <el-form ref="form" :model="form" class="form-home">
                    <div class="flex">
                      <el-input
                        v-model="form.email"
                        class="input-home"
                        placeholder="Enter your email"
                        clearable
                      />
                      <el-button type="primary">Sign Up</el-button>
                    </div>
                  </el-form>
                </el-col>
              </el-row>
              <div class="text-center no-credit">No credit card required</div>
            </div>
          </el-container>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        email: ''
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.wide {
  font-size: 30px;
  margin-bottom: 20px;
}

.no-credit {
  font-size: 12px;
  color: var(--main-text-color);
  padding-top: 10px;
}
</style>
