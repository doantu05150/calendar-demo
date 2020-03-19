<template>
  <div>
    <section>
      <div class="sub-section">
        <div class="container">
          <el-container>
            <div class="w-full">
              <div class="font-bold h-title wide w-full">
                How it work
              </div>
              <el-row class="step">
                <el-col :span="12">
                  <img
                    src="https://assets.calendly.com/assets/landing/homepage/availability-c2da8e58b71054d8eae714114ecee32c5653257f929210ef11a4c0f614164c2b.png"
                    class="img-fluid img-s1"
                    alt="step1"
                  />
                </el-col>
                <el-col :span="12">
                  <div class="description">
                    <div class="h-title wide-t font-bold">
                      Create simple rules
                    </div>
                    <p>
                      Setup is easy. Let Calendly know your availability
                      preferences and it’ll do the work for you.
                    </p>
                  </div>
                </el-col>
              </el-row>
              <el-row class="step m-0auto">
                <el-col :span="12">
                  <img
                    src="https://assets.calendly.com/assets/landing/homepage/linking-b6a9a582d012421366302256c668eaf3cd88d7d8a1b1e8fa19e96bcb8ff2ea85.png"
                    class="img-fluid img-s1"
                    alt="step1"
                  />
                </el-col>
                <el-col :span="12">
                  <div class="description">
                    <div class="h-title wide-t font-bold">
                      Share your link
                    </div>
                    <p>
                      Share your Calendly links via email or embed it on your
                      website.
                    </p>
                  </div>
                </el-col>
              </el-row>
              <el-row class="step float-right clearfix mb-0">
                <el-col :span="12">
                  <img
                    src="https://assets.calendly.com/assets/landing/homepage/booking-f274b2610c18540634cc9ab7210256b0fc582ffd01a444b328afaa93b4c88526.png"
                    class="img-fluid img-s1"
                    alt="step1"
                  />
                </el-col>
                <el-col :span="12">
                  <div class="description">
                    <div class="h-title wide-t font-bold">
                      Schedule
                    </div>
                    <p>
                      They pick a time and the event is added to your calendar.
                    </p>
                  </div>
                </el-col>
              </el-row>
            </div>
          </el-container>
        </div>
      </div>
    </section>
  </div>
</template>

<style lang="scss" scoped>
.wide {
  padding-bottom: 20px;
  font-size: 30px;
  text-align: center;
}

.wide-t {
  font-size: 18px;
}

.description {
  p {
    color: var(--main-text-color);
    margin-top: 0 !important;
  }
}

.step {
  max-width: 620px;
  margin-bottom: 65px;
}

.img-s1 {
  min-width: 300px;
  min-height: 225px;
}
</style>
