<template>
  <div id="app">
    <el-row>
      <el-col>
        <el-input :type="text" placeholder="Please input" v-model="input" :tabindex="0" >
          <span slot="prefix">prefix</span>
          <span slot="suffix">suffix</span>
          <span slot="prepend">prepend</span>
          <span slot="append">append</span>
        </el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row>
      <el-col :span="12"><div class="content">hoge</div></el-col>
      <el-col :span="12"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :span="16"><div class="content">hoge</div></el-col>
      <el-col :span="8"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :span="4"><div class="content">hoge</div></el-col>
      <el-col :span="8"><div class="content">hoge</div></el-col>
      <el-col :span="4"><div class="content">hoge</div></el-col>
      <el-col :span="4"><div class="content">hoge</div></el-col>
      <el-col :span="4"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6" :offset="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :span="2" :offset="4"><div class="content">hoge</div></el-col>
      <el-col :span="6" :offset="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row type="flex">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row type="flex" justify="center">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row type="flex" justify="end">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row type="flex" justify="space-between">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row type="flex" justify="space-around">
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
      <el-col :span="6"><div class="content">hoge</div></el-col>
    </el-row>
    <el-row :gutter="20">
      <el-col :xs="8" :sm="6" :md="4" :lg="3" :xl="1"><div class="content">hoge</div></el-col>
      <el-col :xs="4" :sm="6" :md="8" :lg="9" :xl="11"><div class="content">hoge</div></el-col>
      <el-col :xs="4" :sm="6" :md="8" :lg="9" :xl="11"><div class="content">hoge</div></el-col>
      <el-col :xs="8" :sm="6" :md="4" :lg="3" :xl="1"><div class="content">hoge</div></el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'layout',
  data() {
    return {
      inpit: ''
    }
  }
}
</script>

<style>
.el-row {
  margin-bottom: 10px;
}
.content {
  background-color: lightgray;
  border-radius: 5px;
}
</style>


