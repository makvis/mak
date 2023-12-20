<script lang="ts">
import { Vue, Component } from "vue-property-decorator";
@Component({})
export default class HeaderComponent extends Vue {}
</script>
<template>
  <el-header height="auto">
    <el-row type="flex" class="row-bg" justify="space-between">
      <el-col class="header-logo" :span="12">
        <a href="#">  <!--все картинки в папке assets*/ -->
            <img src="@/assets/img/log.jpg" alt="logo" />
        </a>
      <el-col :span="12"
        ><div>
          <el-menu :default-active="activeIndex" mode="horizontal">
            <el-menu-item index="1">Processing Center</el-menu-item>
            <el-menu-item index="3" disabled>Info</el-menu-item>
            <el-menu-item index="4"></el-menu-item>
          </el-menu></div
      ></el-col>
    </el-row>
  </el-header>
</template>
<style lang="scss" scroped></style>
