<template>
  <div>
    <div class="footer m-0auto">
      <el-row :gutter="24" align="middle">
        <el-col :span="12">
          <a href="#">
            <img
              src="https://assets.calendly.com/assets/landing/logo_icon-5855fd7f1e3a31267dbb103936ea0db589e06132b13bf2086048a1020d764e3f.png"
              class="ft-logo"
              alt="logo"
            />
          </a>
        </el-col>
        <el-col :span="12">
          <div class="flex justify-fend">
            <el-dropdown class="ct-dropdown">
              <span class="el-dropdown-link">
                Language
              </span>
              <el-dropdown-menu slot="dropdown">
                <el-dropdown-item>Vietnam</el-dropdown-item>
                <el-dropdown-item icon="el-icon-check"
                  >English</el-dropdown-item
                >
              </el-dropdown-menu>
            </el-dropdown>
          </div>
        </el-col>
      </el-row>
    </div>
    <hr class="footer-line-break" />
    <div class="footer m-0auto">
      <el-row :gutter="24" align="middle">
        <el-col :span="18">
          <div>
            <el-row>
              <el-col
                v-for="(row, index1) in footer"
                :key="`row_${index1}`"
                :span="6"
              >
                <div
                  v-for="(col, index2) in row"
                  :key="`col_${index2}`"
                  class="column"
                >
                  <div class="ft-title">{{ col.title }}</div>
                  <ul class="ft-ul">
                    <li
                      v-for="(item, index3) in col.list"
                      :key="`item_${index3}`"
                      class="ft-li"
                    >
                      {{ item.title }}
                    </li>
                  </ul>
                </div>
              </el-col>
            </el-row>
          </div>
        </el-col>
        <el-col :span="6">
          <div class="flex justify-fend">
            <div class="column text-left">
              <div class="ft-title">Download our app</div>
              <img
                src="https://assets.calendly.com/assets/landing/en/footer/apple-app-store-91611e84d781e99b8716b25eb292d53cfe0e78f66d07473e08dfec595c717673.svg"
                alt="app"
              />
            </div>
          </div>
        </el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      footer: [
        [
          {
            title: 'Product',
            list: [
              {
                title: 'Features',
                link: '#'
              },
              {
                title: 'Integrations',
                link: '#'
              },
              {
                title: 'For Teams',
                link: '#'
              }
            ]
          },
          {
            title: 'Pricing',
            list: [
              {
                title: 'Plans',
                link: '#'
              }
            ]
          }
        ],
        [
          {
            title: 'Product',
            list: [
              {
                title: 'Features',
                link: '#'
              },
              {
                title: 'Integrations',
                link: '#'
              },
              {
                title: 'For Teams',
                link: '#'
              }
            ]
          }
        ],
        [
          {
            title: 'Product',
            list: [
              {
                title: 'Features',
                link: '#'
              },
              {
                title: 'Integrations',
                link: '#'
              },
              {
                title: 'For Teams',
                link: '#'
              }
            ]
          }
        ],
        [
          {
            title: 'Product',
            list: [
              {
                title: 'Features',
                link: '#'
              },
              {
                title: 'Integrations',
                link: '#'
              },
              {
                title: 'For Teams',
                link: '#'
              }
            ]
          }
        ]
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.footer {
  max-width: var(--footer-width);
}

.ft-logo {
  width: 38px;
}

.ct-dropdown {
  border: 1px solid #606266;
  padding: 8px 36px;
  border-radius: 4px;
}

.footer-line-break {
  border-top: 1px solid #ececec;
  margin: 10px 0 30px;
}

.ft-title {
  font-size: 18px;
  margin-bottom: 15px;
  color: #444752;
  font-family: 'Baloo Chettan 2', cursive;
  font-weight: 600;
  padding-top: 6px;
}

.ft-ul {
  list-style: none;
  padding: 0;
}

.ft-li {
  padding: 0;
  font-size: 16px;
  font-family: 'Baloo Chettan 2', cursive;
  font-weight: 400;
  color: #525252;
  padding: 2px 0;
}
</style>
