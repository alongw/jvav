<script setup lang="ts">
// import here ...

defineOptions({
  name: 'UnderComponent'
})

// code here ...
</script>

<template>
  <div class="under">
    <ul>
      <li>© ZhangHaoYang</li>
      <li>选择语言</li>
      <li>支持</li>
      <li>隐私政策</li>
      <li>Cookie</li>
      <li>喜好设置</li>
      <li>使用条款</li>
      <li>商标</li>
    </ul>
  </div>
</template>

<style scoped lang="less">
.under {
  height: 110px;
  background-color: #eeeeee;
  ul {
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    li {
      cursor: pointer;
      margin: 5px;
      font-size: 10px;
      color: #2d5986;
      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>
