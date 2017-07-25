<template>
  <div id="editor">
    <div class="select-person">
      <h2>选择人员</h2>
      <el-select v-model="value" placeholder="请选择" class="select">
        <el-option v-for="item in persons" :key="item.value" :label="item.label" :value="item.value">
        </el-option>
      </el-select>
    </div>
    <div class="select-person">
      <el-button type="primary" class="button">新增人员</el-button>
      <el-input placeholder="请输入人员姓名" class="input"></el-input>
    </div>
    <div class="input-area">
      <ul class="type">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-study"></use>
        </svg>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'preview',
  data() {
    return {
      persons: [{
        value: '阳哥',
        label: '阳哥'
      }, {
        value: '周杰伦',
        label: '周杰伦'
      }, {
        value: '斯琴高娃',
        label: '斯琴高娃'
      }],
      value: ''
    }
  }
}
</script>

<style lang="stylus">
  #editor
    display: flex
    flex-direction: column
    width: 300px
    margin: 0 25px 0 0
    border: 1px solid #ddd
    border-radius: 10px
    background-color: #fff
    .select-person
      display: flex
      line-height: 40px
      justify-content: center
      align-items: center
      margin: 10px 0
      h2
        width: 88px
        text-align: center
      .select, .input
        width: 160px
        margin-left: 10px
      .button
        height: 36px
    .input-area
      flex-grow: 1
</style>