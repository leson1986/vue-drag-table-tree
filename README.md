# vue drag tree table

IE11+/Chrome/firefox

## 请更新到```1.0.2```及以上版本
> 基于vue实现的可以拖拽排序的树形表格   

支持拖拽排序、固定头、拖拽改变行宽，checkbox多选、自定义单元格内容、设置行的背景色、动态控制某些行是否可以拖拽等等....

![drag-tree-table]('vue-dragTree-table')

## 安装
npm
``` bashs
npm i vue-drag-table-tree --save-dev
```
script
``` bashs
<script src="./dist/dtree-table.js"></script>
```
## 使用方式

```html
<template>
  <div id="app">
    <dragTreeTable
      :data="treeData"
      :onDrag="onTreeDataChange"
      fixed
      border>
    </dragTreeTable>
  </div>
</template>

<script>
import dragTreeTable from "drag-tree-table";
export default {
  name: "app",
  data() {
    return {
      treeData: {
        columns: [...],
        lists: [...]
      }
    };
  },
  components: {
    dragTreeTable
  },
  methods: {
    onTreeDataChange(list) {
      this.treeData.lists = list;
    }
  },
};
</script>

```
[更新日志-CHANGELOG](CHANGELOG.md 'vue-drag-table-tree')

## 我的扣扣```511539312```，欢迎沟通（找我加新需求的记得先来个star支持下哦）
