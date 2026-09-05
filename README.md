# GoldMiner‑Game
> Android 版本黄金矿工游戏，基于 libGDX 跨平台游戏框架开发

## 中文介绍
本项目是**黄金矿工（GoldMiner）** 的安卓移植版本。项目以开源仓库 [GoldMiner_Game_FullSourceCode](https://github.com/nguyenquanghuy15091995/GoldMiner_Game_FullSourceCode.git) 的游戏源码作为基础，升级迁移至现代 `gdx‑liftoff` 脚手架生成的全新 libGDX 工程框架。

项目采用标准多模块跨平台结构：
- **core**：存放全部游戏核心业务逻辑、游戏资源，代码可以在安卓、桌面等多个平台共用；
- **lwjgl3**：桌面端（PC）运行入口；
- **android**：安卓移动端适配模块，完成安卓系统的兼容、资源打包、应用启动。

游戏实现经典黄金矿工玩法：玩家操控吊钩抓取金矿、钻石等宝物，避开石块等障碍物，在限定时间内达成目标金额即可通关。本次升级重构了旧版工程结构，修复了安卓端图片资源加载失败、文件路径异常等兼容性问题，适配新版 Android SDK，可直接在安卓模拟器与实体手机上运行。

## 构建

如果你想从源代码构建，只需

    git clone --recursive https://github.com/Margarithuang/GoldMiner_Game-Android.git
    git submodule update --init --recursive
    ./gradlew build

## 运行说明 / How to run
1. 导入项目至 Android Studio
2. 同步 Gradle
3. 选择 `android` 运行配置，启动安卓模拟器或连接安卓真机，点击运行即可
