<template>
  <div class="hello">
    <el-carousel :interval="10000" type="card" height="600px">
      <el-carousel-item v-for="item in 6" :key="item">
        <h3>{{ item }}</h3>
      </el-carousel-item>
    </el-carousel>
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
          <el-col :span="8">
            <div class="grid-content learn">
              <el-button>了解更多</el-button>
            </div>
          </el-col>
        </el-row>

        
        <el-row>
          <el-col :span="8">
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
          <el-col :span="8">
            <div class="grid-content">
              <el-button>了解更多</el-button>
            </div>
          </el-col>
        </el-row>

      </el-main>
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

.el-carousel {
  background: black;
}

.el-carousel__item h3 {
    color: #475669;
    font-size: 14px;
    opacity: 0.75;
    line-height: 200px;
    margin: 0;
  }
  
  .el-carousel__item:nth-child(2n) {
    background-color: #99a9bf;
  }
  
  .el-carousel__item:nth-child(2n+1) {
    background-color: #d3dce6;
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
    margin: 0 10%;
  }
  .el-button {
    margin: 80px auto;
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
  .learn {

  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }

a {
  color: #42b983;
}
</style>
