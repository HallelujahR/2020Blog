<template>
  <div id="app">

    <el-container>
      <el-header>
        <Nav></Nav>
      </el-header>
      <el-container style="width:1100px;margin:0 auto;border:1px solid blue;">
        <el-main>
          <router-view />
        </el-main>
        <el-aside width="250px">Aside</el-aside>
      </el-container>
    </el-container>

  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0 auto;
  padding: 0px;
}

.el-header {
  color: #333;
  text-align: center;
  line-height: 60px;
  box-shadow: 0 1px 3px rgba(26, 26, 26, 0.1);
  background-clip: content-box;
  margin-bottom: 20px;
}

.el-aside {
  color: #333;

  text-align: center;
  line-height: 200px;
  border: 1px solid pink;
}

.el-main {
  border: 1px solid red;
  padding: 0px;
  margin-right: 20px;
}

body > .el-container {
  margin-bottom: 40px;
  width: 1000px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
