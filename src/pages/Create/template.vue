<template>
  <div id="create">
    <h1>创建文章</h1>
    <h3>文章标题</h3>
    <el-input v-model="title"></el-input>
    <p class="msg">限{{count1}}个字</p>
    <h3>内容简介</h3>
    <el-input type="textarea" v-model="description" :autosize="{ minRows: 2, maxRows: 6}"></el-input>
    <p class="msg">限{{count2}}个字</p>
    <h3>文章内容</h3>
    <el-input type="textarea" v-model="content" :autosize="{ minRows: 2, maxRows: 30}"></el-input>
    <p class="msg">限{{count3}}个字</p>
    <p>
      <label for="">是否展示到首页</label>
      <el-switch v-model="atIndex" active-color="#13ce66" inactive-color="#ccc"></el-switch>
    </p>
    <el-button type="primary" plain @click="onCreate">确定</el-button>
  </div>
</template>

<script src="./template.js"></script>

<style src="./template.less" lang="less"></style>

