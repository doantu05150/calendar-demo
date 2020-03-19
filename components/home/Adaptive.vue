<template>
  <div>
    <section>
      <div class="sub-section">
        <div class="container">
          <el-container>
            <el-row type="flex" class="row-bg w-full">
              <el-col :span="12">
                <div />
                <div class="font-bold title">
                  Calendly helps you schedule meetings without the
                  back-and-forth emails
                </div>
                <el-form ref="form" :model="form" class="form-home">
                  <div class="flex">
                    <el-input
                      v-model="form.email"
                      class="input-home"
                      placeholder="Enter your email"
                      clearable
                    />
                    <el-button type="primary" @click="onSubmit"
                      >Sign Up</el-button
                    >
                  </div>
                </el-form>
                <div class="text-center des">
                  Get started for free. No credit card required.
                </div>
              </el-col>
              <el-col :span="12">
                <img
                  src="https://assets.calendly.com/assets/landing/homepage/hero-c7322cf6fde0bb0e852c466af957fd7330c8e8607dfe0854947a3cc00a5dfa77.png"
                  alt="hoem-a"
                  class="img-fluid"
                />
              </el-col>
            </el-row>
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
  },
  methods: {
    onSubmit() {}
  }
}
</script>

<style lang="scss" scoped>
.title {
  padding-top: 40px;
  line-height: 36px;
  color: #444752;
  font-family: 'Baloo Chettan 2', cursive;
  font-size: 30px;
  letter-spacing: 0.2px;
}

.des {
  font-size: 14px;
  color: #5a5a5a;
  margin: 10px 0 5px 0;
  padding-bottom: 10px;
  letter-spacing: 1px;
}

.form-home {
  margin-top: 25px;
}
</style>
