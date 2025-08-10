<template>
  <div class="container">
    <!-- 顶部标题栏 -->
    <header class="header">
      <h1>焦作市交通拥挤治理系统</h1>
    </header>

    <div class="content">
      <!-- 左侧功能菜单 -->
      <aside class="sidebar">
        <h3>地图展示</h3>
        <ul>
          <li>二维地图</li>
          <li>基本缩放平移</li>
          <li>物品属性与关联图</li>
          <li>实时路况</li>
          <li>历史热力图</li>
          <li>路段拥堵情况</li>
        </ul>

        <h3>查询功能</h3>
        <ul>
          <li>输入起终点计算路线</li>
          <li>定位并显示信息</li>
          <li>当前天气情况</li>
        </ul>

        <h3>交通治理</h3>
        <ul>
          <li>视频监控 AI 分析</li>
          <li>事故高发地图</li>
          <li>智能信号灯模拟</li>
        </ul>
      </aside>

      <!-- 中间地图区域 -->
      <main class="main">
        <div class="map-placeholder">
          <p>地图/三维模型<br />显示区域<br />(Demo)</p>
        </div>
      </main>

      <!-- 右侧信息栏 -->
      <aside class="sidebar right">
        <h3>信息展示</h3>
        <ul>
          <li>路线规划结果</li>
          <li>实时路况</li>
          <li>天气情况</li>
          <li>监控统计</li>
        </ul>
      </aside>
    </div>
  </div>
</template>

<script setup lang="ts">
// 这里后面可以引入地图 API 和交互逻辑
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  display: flex;
  flex-direction: column;
  height: 100vh;
  font-family: sans-serif;
}

.header {
  background-color: #2f4050;
  color: white;
  padding: 10px;
  text-align: center;
}

.content {
  display: flex;
  flex: 1;
}

.sidebar {
  width: 20%;
  background-color: #f4f7f8;
  padding: 10px;
  overflow-y: auto;
}

.sidebar h3 {
  margin-top: 15px;
  font-size: 14px;
  border-bottom: 1px solid #ccc;
  padding-bottom: 4px;
}

.sidebar ul {
  list-style: none;
  padding-left: 10px;
}

.sidebar ul li {
  margin: 6px 0;
  font-size: 13px;
}

.main {
  flex: 1;
  background-color: #c4c9cd;
  display: flex;
  align-items: center;
  justify-content: center;
}

.map-placeholder {
  text-align: center;
  font-size: 14px;
  color: #333;
}

.right {
  width: 20%;
}
</style>
