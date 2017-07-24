<template>
  <div id="editor">
    <div class="select-person">
      <h2>选择人员</h2>
      <el-select v-model="value" placeholder="请选择" class="select">
        <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value">
        </el-option>
      </el-select>
    </div>
  </div>
</template>

<script>
export default {
  name: 'preview',
  data() {
    return {
      options: [{
        value: '选项1',
        label: '黄金糕'
      }, {
        value: '选项2',
        label: '双皮奶'
      }, {
        value: '选项3',
        label: '蚵仔煎'
      }, {
        value: '选项4',
        label: '龙须面'
      }, {
        value: '选项5',
        label: '北京烤鸭'
      }],
      value: ''
    }
  }
}
</script>

<style lang="stylus">
  #editor
    width: 300px
    margin: 0 25px 0 0
    border: 1px solid #ddd
    border-radius: 10px
    background-color: #fff
    .select-person
      display: flex
      line-height: 40px
      justify-content: center
      margin: 10px 0
      .select
        width: 160px
        margin-left: 10px
</style>