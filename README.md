# Color Picker

> 基于 [farbtastic](https://github.com/mattfarina/farbtastic) 的 jQuery 颜色选择器插件，支持色轮取色与实时预览。

## 简介

一个轻量级的 jQuery 颜色选择器组件，通过色轮（color wheel）让用户直观地选取颜色，选取结果实时同步到关联的 input 框。适合后台管理系统中需要颜色配置的场景（如主题色、标签色等）。

## 功能特性

- 色轮可视化取色，支持色相与明度调节
- 与 input 框双向绑定，实时显示选中颜色的 HEX 值
- 轻量，仅依赖 jQuery
- 样式可自定义

## 依赖

- jQuery 1.10.2+
- jquery-migrate 1.2.1（兼容旧版 API）

## 快速开始

### 1. 引入依赖文件

```html
<link rel="stylesheet" href="./static/public/css/colorpicker.css">
<script src="./static/public/js/jquery1.10.2.js"></script>
<script src="./static/public/js/jquery-migrate1.2.1.js"></script>
<script src="./static/public/js/colorpicker.js"></script>
```

### 2. HTML 结构

```html
<input type="text" id="color" value="#1b2bc5" />
<div id="picker"></div>
```

### 3. 初始化

```javascript
$(document).ready(function() {
  $('#picker').farbtastic('#color');
});
```

`farbtastic()` 的参数为目标 input 的选择器，选取颜色时会自动更新该 input 的值。

## 目录结构

```
.
├── index.htm              # 使用示例页面
└── static/
    └── public/
        ├── js/
        │   ├── jquery1.10.2.js
        │   ├── jquery-migrate1.2.1.js
        │   └── colorpicker.js    # 核心插件
        └── img/
            └── colorpicker/      # 色轮图片资源
```

## 示例

打开 `index.htm` 即可查看颜色选择器的运行效果。

## 相关链接

- farbtastic 原项目：https://github.com/mattfarina/farbtastic
- jQuery 官方文档：https://api.jquery.com/
