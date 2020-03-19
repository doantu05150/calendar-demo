<template>
  <div>
    <section>
      <div class="sub-section">
        <div class="container">
          <el-container>
            <div class="v-wrapper w-full">
              <el-row type="flex" class="row-bg w-full">
                <el-col :span="12">
                  <div class="font-bold h-title wide">
                    Watch our video
                  </div>
                  <p class="vp">
                    We take the work out of connecting with others so you can
                    accomplish more. Learn how painless scheduling can be with
                    Calendly.
                  </p>
                </el-col>
                <el-col :span="12">
                  <div class="flex justify-fend w-full">
                    <iframe
                      src="https://www.youtube.com/embed/URVcea7Si7w"
                      class=""
                      frameborder="0"
                      allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
                      allowfullscreen
                    >
                      Sorry, your browser doesn't support embedded
                      videos.</iframe
                    >
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
.v-wrapper {
  margin-top: 20px;
  padding: 30px 40px;
  border-radius: 3px;
  background-color: #f3faff;
}

.wide {
  font-size: 22px;
  margin-bottom: 10px;
}

.vp {
  color: var(--main-text-color);
}
</style>
