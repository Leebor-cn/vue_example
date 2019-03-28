<template>
  <div id="app">
    <el-container>
      <el-header class="header">
        <vheader></vheader>
      </el-header>
      <el-container class="main">
        <el-aside width="220px" class="aside-menu">
          <navmenu></navmenu>
        </el-aside>
        <el-container>
          <el-main>Main</el-main>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import NavMenu from '@/components/NavMenu'
import Header from '@/components/Header'
export default {
  name: 'app',
  components: {
    'navmenu': NavMenu,
    'vheader': Header
  }
}
</script>

<style>
.header {
  background-color: #409EFF;
  color: #fff;
  line-height: 60px;
}

html body .app .main .aside-menu {
  height: 100%;
}

</style>
