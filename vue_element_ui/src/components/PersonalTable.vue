<template>
  <div>
    <el-container>
      <el-row>
        <el-col :span="2">
            <el-aside>
              <div class="aside-menu">
                  <el-menu>
                      <el-menu-item index="4">
                        <i class="el-icon-setting"></i>
                        <span slot="title">导航四</span>
                      </el-menu-item>
                  </el-menu>
              </div>

            </el-aside>
        </el-col>

        <el-col :span="20">
            <el-main style="padding: 0px;">
              <el-table
                :data="tableData"
                style="width: 100%;">
                <el-table-column
                  prop="ip"
                  label="日期"
                  width="180">
                </el-table-column>
                <el-table-column
                  prop="uptime"
                  label="姓名"
                  width="180">
                </el-table-column>
                <el-table-column
                  prop="diskfree"
                  label="地址">
                </el-table-column>
              </el-table>
            </el-main>
        </el-col>
      </el-row>
    </el-container>

  </div>
</template>


 <script>
    export default {
      name: 'personaltable',
      data() {
        return {
          tableData: [{
            ip : '2016-05-02',
            uptime: '王小虎',
            diskfree: '上海市普陀区金沙江路 1518 弄'
          }, {
            ip: '2016-05-04',
            uptime: '王小虎',
            diskfree: '上海市普陀区金沙江路 1517 弄'
          }]
        }
      }
    }
  </script>
<style>
.aside-menu{
  width: 200px
}


</style>
