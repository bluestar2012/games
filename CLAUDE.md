# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概述

这是一个包含多个经典小游戏的静态 HTML 项目，每个游戏独立存放在各自目录中，均为单文件应用（HTML + CSS + JS 内联）。

## 项目结构

```
games/
├── block/          # 俄罗斯方块 - Tetris with Web Audio API 音效
├── 2048/           # 2048 益智游戏 - 支持键盘和触摸操作
├── 24point/        # 24点游戏 - 算术益智游戏，含求解算法
└── index-backup.html
```

## 运行方式

直接在浏览器中打开对应的 `index.html` 文件即可运行，无需任何构建工具或服务器。

## 技术特点

- **block（俄罗斯方块）**：使用 Canvas 渲染，Web Audio API 生成背景音乐和音效，支持难度选择和本地存储最高分
- **2048**：支持键盘方向键、WASD 以及触摸屏滑动手势，使用 CSS Grid 布局
- **24点**：包含回溯算法 `solve24()` 求解任意 4 个 1-10 数字是否能计算出 24，支持提示功能

## 开发说明

每个游戏目录下的 `index.html` 包含完整的游戏代码（HTML 模板、内联 CSS、内联 JavaScript）。如需修改游戏逻辑，直接编辑对应目录下的 `index.html` 文件即可。
