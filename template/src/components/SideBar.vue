<template>
    <div class="full">
        <el-row class="full">
            <el-col :span="4" class="full-height" >
                <el-menu default-active="2" class="el-menu-vertical-demo full-height">
                    <el-submenu index="1" >
                        <template slot="title"><i class="el-icon-message"></i>导航一</template>
                        <el-menu-item-group>
                            <template slot="title">分组一</template>
                            <router-link to="/baseForm" tag="li"><el-menu-item index="1-1">基本表单</el-menu-item></router-link>
                            <el-menu-item index="1-2">选项2</el-menu-item>
                        </el-menu-item-group>
                        <el-menu-item-group title="分组2">
                            <el-menu-item index="1-3">选项3</el-menu-item>
                        </el-menu-item-group>
                        <el-submenu index="1-4">
                            <template slot="title">选项4</template>
                            <el-menu-item index="1-4-1">选项1</el-menu-item>
                        </el-submenu>
                    </el-submenu>
                    <el-menu-item index="2"><i class="el-icon-menu"></i>导航二</el-menu-item>
                    <el-menu-item index="3"><i class="el-icon-setting"></i>导航三</el-menu-item>
                </el-menu>
            </el-col>
            <el-col :span="20" style="padding: 10px 30px 10px 10px"><router-view></router-view></el-col>
        </el-row>
    </div>
</template>

<script>
</script>

<style  scoped>
    .sidebar{
        background-color: #324056;
    }
</style>
