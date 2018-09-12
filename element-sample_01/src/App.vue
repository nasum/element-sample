<template>
  <div id="app">
    <el-row>
      <el-col>
        <el-input-number v-model="num" :min="1" :max="100" :precision="2" size="large"></el-input-number>
        <el-input-number v-model="num" :min="1" :max="100" :precision="2" size="medium"></el-input-number>
        <el-input-number v-model="num" :min="1" :max="100" :precision="2" size="small"></el-input-number>
        <el-input-number v-model="num" :min="1" :max="100" :precision="2" size="mini"></el-input-number>
      </el-col>
    </el-row>
    <el-row>
      <el-col>
        <el-input-number v-model="num" :min="1" :max="100" :precision="2" size="large" :controls="true"></el-input-number>
        <el-input-number v-model="num" :min="1" :max="100" :precision="2" size="medium" :controls="false"></el-input-number>
      </el-col>
    </el-row>
    <el-row>
      <el-col>
        <el-select v-model="valueArray" placeholder="Select" size="large" :clearable="true" :multiple="true" :collapse-tags="true" filterable allow-create>
          <el-option
            v-for="item in options"
            :key="item.value"
            :label="item.label"
            :value="item.value">
          </el-option>
        </el-select>
        <el-select v-model="value" placeholder="Select" size="medium" :filterable="true">
          <el-option
            v-for="item in options"
            :key="item.value"
            :label="item.label"
            :value="item.value">
          </el-option>
        </el-select>
        <el-select v-model="value" placeholder="Select" size="small">
          <el-option
            v-for="item in options"
            :key="item.value"
            :label="item.label"
            :value="item.value">
          </el-option>
        </el-select>
        <el-select v-model="value" placeholder="Select" size="mini">
          <el-option
            v-for="item in options"
            :key="item.value"
            :label="item.label"
            :value="item.value">
          </el-option>
        </el-select>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'layout',
  data() {
    return {
      num: 0,
      options: [{
        value: 'Option1',
        label: 'Option1'
      }, {
        value: 'Option2',
        label: 'Option2'
      }, {
        value: 'Option3',
        label: 'Option3'
      }, {
        value: 'Option4',
        label: 'Option4'
      }, {
        value: 'Option5',
        label: 'Option5'
      }],
      value: '',
      valueArray: []
    }
  },
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


