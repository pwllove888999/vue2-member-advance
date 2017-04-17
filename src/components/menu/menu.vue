<template lang="html">
  <div class="menu">
    <el-menu default-active="1" @open="handleOpen" @close="handleClose">
       <el-submenu index="1">
         <template slot="title"><i class="el-icon-message"></i>首页</template>
         <el-menu-item index="1-1">选项1</el-menu-item>
         <el-menu-item index="1-2">选项2</el-menu-item>
         <el-menu-item index="1-3">选项3</el-menu-item>
         <el-menu-item index="1-4">选项4</el-menu-item>
       </el-submenu>
       <el-submenu index="2">
         <template slot="title"><i class="el-icon-menu"></i>会员管理</template>
         <el-menu-item index="2-1">主页</el-menu-item>
         <el-menu-item index="2-2">个人中心</el-menu-item>
       </el-submenu>
       <el-submenu index="3">
         <template slot="title"><i class="el-icon-setting"></i>导航三</template>
         <el-menu-item index="3-1">选项1</el-menu-item>
         <el-menu-item index="3-2">选项2</el-menu-item>
       </el-submenu>
     </el-menu>
  </div>
</template>

<script>
export default {
  methods: {
    handleOpen (key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style lang="sass" scoped>
// 菜单栏的宽度
$menuWidth: 200px

.menu
  position: absolute
  width: $menuWidth
  // background: #f60
  color: #fff
</style>
