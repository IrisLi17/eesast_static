<template>
  <div class="hello">
    <el-container>
      <el-aside width="30%">
        <h2>我们的部门</h2>
        <el-card class="box-card">
          <div>
            <i class="el-icon-document"></i>
            <p>网宣部</p>
          </div>
        </el-card>
        <el-card class="box-card">
          <div>
            <i class="el-icon-document"></i>
            <p>软件部</p>
          </div>
        </el-card>
        <el-card class="box-card">
          <div>
            <i class="el-icon-document"></i>
            <p>硬件部</p>
          </div>
        </el-card>
        <el-card class="box-card">
          <div>
            <i class="el-icon-document"></i>
            <p>学培部</p>
          </div>
        </el-card>
        <el-card class="box-card">
          <div>
            <i class="el-icon-document"></i>
            <p>项目部</p>
          </div>
        </el-card>
      </el-aside>

      <el-main>

        <el-row>
          <el-col :span="16">
            <div class="grid-content light-blue">
              <div class="theme-disc">
                <h3>讲座</h3>
                <p>讲座</p>
              </div>
              <img src="../assets/logo.png">
            </div>
          </el-col>
          <el-col :span="6">
            <div class="grid-content">
              <el-button>了解更多</el-button>
            </div>
          </el-col>
        </el-row>

        
        <el-row>
          <el-col :span="6">
            <div class="grid-content">
              <el-button>了解更多</el-button>
            </div>
          </el-col>
          <el-col :span="16">
            <div class="grid-content light-blue">
              <img src="../assets/logo.png">
              <div class="theme-disc">
                <h3>活动</h3>
                <p>活动</p>
              </div>
              
            </div>
          </el-col>
        </el-row>

        <el-row>
          <el-col :span="16">
            <div class="grid-content light-blue">
              <div class="theme-disc">
                <h3>SAST WEEKLY</h3>
                <p>SAST WEEKLY</p>
              </div>
              <img src="../assets/logo.png">
            </div>
          </el-col>
          <el-col :span="6">
            <div class="grid-content">
              <el-button>了解更多</el-button>
            </div>
          </el-col>
        </el-row>


        <h1>{{ msg }}</h1>
      </el-main>
    </el-container>
    <el-container>
      <el-footer>
      </el-footer>
  </el-container>
  </div>
</template>

<script>
export default {
  name: 'Index',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("//unpkg.com/element-ui@2.3.4/lib/theme-chalk/index.css");

h1, h2 {
  font-weight: normal;
}
i {
  width: 50px;
}
.box-card {
  width: 80%;
  margin: 0 auto;
}
.el-row {
    margin-bottom: 20px;
  }
  .el-col {
    border-radius: 4px;
  }
  .el-col img {
    max-width: 30%;
    margin: 0 10%;
    padding: 0;
  }
  .el-button {
    margin: 30% auto;
  }
  .light-blue {
    background: rgb(104,202,255,0.3);
  }
  .theme-disc {
    align-items: center;
    margin: 0 auto;
    padding: 0;
  }
  .grid-content {
    display:flex;
    border-radius: 4px;
    min-height: 36px;
    align-items: center;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }

a {
  color: #42b983;
}
</style>
