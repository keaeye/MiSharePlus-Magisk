# MiShare 合成版 Magisk 模块

## 模块简介
本模块集成了 **MiShare（小米互传）功能模块** 与 **Miui Core 框架模块**，使非小米手机也能正常运行小米互传功能，无需复杂配置，安装即用。

通过合并两个核心组件，该模块能够：
- 支持非小米设备使用 **MiShare 小米互传功能**
- 提供运行小米相关应用所需的 **MIUI 框架支持**
- 无需依赖原系统环境，提升兼容性与稳定性

适用于希望使用小米互传功能的所有 Android 设备用户。

---

## 功能特点
- 支持小米互传的核心服务与后台组件
- 内置 MIUI 框架依赖（`miui`, `com.miui.core`, `com.miui.system`, `com.miui.rom` 等）
- 自动挂载并提供小米互传 App（包含在模块中）
- 使用 Magisk 或 KernelSU 挂载方式，不改写系统分区
- 可搭配其他 MIUI 系应用（如小米相册、小米文件管理器等）使用

---

## 系统要求
- 设备 **非 MIUI 系统**（如 Pixel、三星、类 AOSP 系 ROM）
- 支持架构：`arm64-v8a` 或 `armeabi-v7a`
- Android 版本 **≥ 5.0（SDK 21）**
- 已安装 **Magisk** 或 **KernelSU**

---

## 安装指南
1. 使用 **Magisk App、KernelSU App** 或 **Recovery** 安装模块 ZIP 文件  
2. 如果使用 **KernelSU**，请：
   - 打开 KernelSU 设置
   - **默认禁用 Unmount Modules**
3. 启动系统后，**从桌面或应用抽屉中手动打开“小米互传” App**
   - 首次启动将自动申请必要权限（蓝牙、Wi-Fi、位置等），请全部授予
4. 如使用 KernelSU，还需：
   - 手动授予 `package.txt` 中列出的所有包名的超级用户权限（启用“显示系统应用”）
   - 然后重新启动一次设备
5. 若使用其他依赖该模块的 Miui App 模块，也请按需一并安装

---

## 下载地址
[👉 前往 GitHub Releases 页面下载最新版本](https://github.com/keaeye/MiSharePlus-Magisk/releases)

---

## 免责声明
- 小米互传及 MIUI 框架组件版权归 Xiaomi™ 所有
- 本模块仅为研究与个人学习用途，请勿用于商业行为
- 模块中 Magisk 安装脚本及合并逻辑遵循 MIT 协议，其余 App 组件请遵守其原版权要求
