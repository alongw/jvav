<script setup lang="ts">
// import here ...
import { Search } from '@icon-park/vue-next'

defineOptions({
  name: 'NavComponent'
})

// code here ...
</script>

<template>
  <div class="nav">
    <div class="logo">
      <img src="@/assets/logo.png" alt="" />
    </div>
    <div class="navbar">
      <ul>
        <li>下载</li>
        <li>Developer Resources</li>
        <li>帮助</li>
      </ul>
      <div class="search">
        <div class="input">
          <search theme="outline" size="14" fill="#333" />
          <input type="text" placeholder="搜索" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="less">
.nav {
  display: flex;
  align-items: center;
  height: 80px;
  background-color: #3a75b0;
  padding: 0 15px;
  .logo {
    width: 125px;
    height: 73px;
    img {
      width: 100%;
      height: 100%;
    }
  }

  .navbar {
    display: flex;
    flex: 1;
    justify-content: space-between;
    align-items: center;
    margin-left: 50px;
    padding: 0 25px;
    // background-color: pink;
    ul {
      display: flex;
      li {
        cursor: pointer;
        margin: 10px;
        font-size: 25px;
        color: #fefbf9;
        transition: all 0.3s;

        &:hover {
          color: #e76f00;
        }
      }
    }

    .search {
      .input {
        display: flex;
        align-items: center;
        padding: 0 20px;
        // width: 200px;
        height: 35px;
        background-color: #ffffff;
        border: 1px solid #d6d6e7;
        input {
          width: 150px;
          border: none;
          outline: none;
          margin-left: 5px;
          height: 100%;
          transition: all 0.3s;
          &:focus {
            width: 200px;
          }
        }
      }
    }
  }
}
</style>
