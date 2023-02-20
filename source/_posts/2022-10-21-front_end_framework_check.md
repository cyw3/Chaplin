
---
title: 2022-10-21-front_end_framework_check
date: 2022-10-21 16:20:12
author: yalechen
tags: TCA
toc: true
author_site: https://github.com/cyw3
---

# 腾讯云代码分析 TCA - 前端框架检查规则包

## 背景

前端项目在长期发展过程中，由于框架开源许可证变更、框架性能外观等不适用等因素，需要对前端框架进行平滑切换，而这就需要[腾讯云代码分析 TCA](https://github.com/Tencent/CodeAnalysis) 的介入，方便对企业内所有前端项目进行批量分析统计，方便管理。

## 需求

- 检查代码仓库中使用到指定前端框架的代码位置。

### 示例

```json
{
  "name": "framework",
  "version": "1.0.0",
  "dependencies": {
    "react": "^17.0.2", // 触发规则
    "react-dom": "^17.0.2", // 触发规则
    "react-hotkeys-hook": "^3.4.3", // 触发规则
    "react-redux": "^7.2.5", // 触发规则
    "single-spa": "^5.9.3",
    "universal-cookie": "^4.0.4"
  },
}
```

## 快速体验

TCA 现已支持前端框架检查规则包，可以在 TCA 分析方案中搜索勾选以下规则包，快速体验。

### 启用规则包
分析方案 -> 代码检查 -> 前端框架检查规则包 -> 启用/查看规则

### 支持框架

- TDesign
- AntD
- React
- Vue


### 更多

更多框架支持，欢迎提 issue 进行咨询扩展。