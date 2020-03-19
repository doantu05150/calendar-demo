<template>
  <div>
    <section>
      <div class="sub-section">
        <div class="container">
          <el-container>
            <div class="w-full">
              <div class="font-bold h-title wide w-full">
                You're in good company
              </div>
              <p class="hp text-center fs">
                We're already connecting millions of people
              </p>
              <div class="huge-ticket">
                <div class="handles" />
                <div class="number">5,000,000</div>
                <div class="units">Monthly Users</div>
              </div>
              <p class="hp text-center fs">
                Trusted by
              </p>
              <div class="flex space-between">
                <div v-for="i in 4" :key="i">
                  <img
                    class="img-fluid"
                    src="https://assets.calendly.com/assets/landing/homepage/linkedin_logo-9b3c8e76c1b73b3bf7a2bd0937001b1b9adbae6331e76eda22f9540fedc292da.png"
                    alt="trusted by"
                  />
                </div>
              </div>
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

.fs {
  font-size: 20px;
}

.huge-ticket {
  font-size: 136px;
  line-height: 230px;
  position: relative;
  margin: 60px 0 40px;
  padding-bottom: 2vw;
  border: #454952 1px solid;
  background-color: #fff;
  text-align: center;
  border-radius: 0.2em;
  font-weight: 600;
  color: var(--main-text-color);

  .handles {
    position: absolute;
    top: -5%;
    left: 10%;
    right: 10%;
    bottom: auto;
    height: 17%;

    &::before {
      content: '';
      position: absolute;
      top: 0;
      left: auto;
      right: auto;
      bottom: 0;
      width: 3%;
      background-color: #fff;
      border: #454952 1px solid;
      border-radius: 11px;
      z-index: 1;
      right: 0;
    }

    &::after {
      content: '';
      position: absolute;
      top: 0;
      left: auto;
      right: auto;
      bottom: 0;
      width: 3%;
      background-color: #fff;
      border: #454952 1px solid;
      border-radius: 11px;
      z-index: 1;
      left: 0;
    }
  }

  &::after {
    content: '';
    position: absolute;
    top: auto;
    left: 2.4%;
    right: 2.4%;
    bottom: -4.8%;
    height: 60px;
    border: inherit;
    border-radius: inherit;
    z-index: -1;
  }

  .units {
    font-size: 20px;
    text-align: center;
    position: absolute;
    left: 0;
    right: 0;
    bottom: 14%;
    height: 0.15em;
    line-height: 0.15em;
    font-size: 0.15em;
    font-weight: bold;
  }
}
</style>
