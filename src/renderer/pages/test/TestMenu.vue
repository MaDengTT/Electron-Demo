<template>
<div id="two-app">
            <el-menu default-active="['1','3']">
              <el-submenu index="1">
                <template slot="title">
                  <i class="el-icon-message">
                    导航一
                  </i>
                </template>
                <el-menu-item-group>
                  <template slot="title">
                    分组一
                    </template>
                  <el-menu-item index="1-1">
                    选项一
                  </el-menu-item>
                  <el-menu-item index="1-2">
                    选项二
                  </el-menu-item>
                </el-menu-item-group>
              </el-submenu>
              <el-menu-item index="2">
                导航二
              </el-menu-item>
            </el-menu>
</div>
</template>