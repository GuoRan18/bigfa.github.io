---
title: "关于主题"
description:
date: 2024-10-10T23:22:50+08:00
cover:
hidden: false
comments: true
---

最近memos更新到了0.26，导致木木老师的Panr主题中哔哔广场不能用了，索性换上了Theme [farallon](https://github.com/bigfa/hugo-theme-farallon) by bigfa 

### 主题修改记录
2024-10-11
- 字体选择[霞鹜文楷](https://github.com/lxgw/LxgwWenKai)
- 样式增加text-align: justify
- H3标签增加样式
- 顶部颜色修改
```
body {
    letter-spacing: 0;
    text-align: justify;
    font: {
        weight: 400;
        style: normal;
        family: "LXGW WenKai Screen", "微软雅黑", "Microsoft YaHei", "Georgia", "STZhongsong", serif;
        size: 16px;
    }
```
```
h3{    font-size: 20px;
    line-height: 1em;
    border-left: 5px solid #ef7c7c;
    font-weight: bold;
    padding: 0px 0 1px 5px;
    margin: 10px 0
}
```
```
.main {
    position: relative;
    &::after {
        aspect-ratio: 1/3;
        background-image: linear-gradient(to right, #007cf0, #d923238a);
        border: 0 solid #e5e5e5;
        border-radius: 9999px;
        bottom: calc(100% - 100px);
        filter: blur(44px);
        opacity: 0.2;
        position: absolute;
        right: 0;
        left: 0;
        //z-index: -50;
        content: "";
    }
}
```