# SmoothScroll Lite

![version](https://img.shields.io/badge/version-1.2.0-blue) ![release](https://img.shields.io/github/v/release/qiukela4-rgb/smoothscroll-lite-app) ![platform](https://img.shields.io/badge/platform-Windows-lightgrey)

Windows 滚轮平滑引擎：把鼠标滚轮刻度拆成亚格脉冲，按 200Hz 节拍投递，
让各类桌面应用得到连续、可调的滚动手感。单文件绿色版，双击即用，托盘常驻。

作者：**nian**（[GitHub @qiukela4-rgb](https://github.com/qiukela4-rgb)）。
源码私有维护，本仓库只提供下载、说明与版本记录。

## 参考项目

- [quangtruong2003/SmoothScroll](https://github.com/quangtruong2003/SmoothScroll) —— 新版 SmoothScroll（1.37.2）的公开项目页。本项目的界面形态与能力设计参考了它的 120Hz 缓动引擎、按应用配置、托盘面板、全局热键与游戏避让；其桌面端源码同样私有维护。

## 下载

- [v1.2.0 单文件 exe](https://github.com/qiukela4-rgb/smoothscroll-lite-app/releases/download/v1.2.0/SmoothScroll-Lite-v1.2.0.exe)
- [全部发布版本](https://github.com/qiukela4-rgb/smoothscroll-lite-app/releases)

## 主要功能

- 三轴引擎：纵向、横向、Ctrl+滚轮缩放；四条缓动曲线（exponential / quintic / cubic / linear）。
- 步长、动画时长、加速上限、脉冲频率实时生效；最大速度、尾首比例、整格 / 亚格 / 原生输出模式。
- 按应用独立参数、高 DPI 折算、游戏模式避让、Windows 自带平滑应用避让。
- 全局快捷键开关平滑；托盘左键双击打开设置，右键自绘面板。
- 设置页含滚动 / 高级 / 游戏模式 / 应用 / 行为 / 关于六页，配置可导入导出。

## 在线更新

程序「关于 → 在线更新」会读取本仓库的 GitHub Releases 接口检查新版本，
启动后 24 小时内最多自动检查一次，也可以手动检查。只提示、不自动下载或替换文件；
断网、超时、限流时显示提示文字，不影响滚动功能。

## 使用说明

双击 exe 后托盘出现图标并弹出设置窗口。关闭窗口只是收进托盘；真正退出走托盘菜单或设置页「退出」。
配置保存在 `%APPDATA%\SmoothScrollLite\config.json`。
本程序与同名平滑滚动工具不能同时开启（两个低层鼠标钩子会互抢事件），启动时会清理冲突进程。
