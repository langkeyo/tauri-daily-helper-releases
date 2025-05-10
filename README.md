# 日报助手发布版本

这个仓库用于存储日报助手应用程序的各平台安装包，包括Windows、macOS和Linux版本。

## 目录结构

- `/windows` - Windows平台安装包
  - `.msi` - Windows安装程序
  - `.exe` - 可执行安装程序
- `/macos` - macOS平台安装包
  - `.dmg` - macOS安装镜像
  - `.app.tar.gz` - 压缩的应用程序包
- `/linux` - Linux平台安装包
  - `.AppImage` - 通用Linux应用程序
  - `.deb` - Debian/Ubuntu安装包

## 发布说明

每个版本的更新信息和下载链接都会在GitHub Releases页面中发布，请访问[Releases页面](https://github.com/langkeyo/tauri-daily-helper-releases/releases)获取最新版本。

## 跨平台构建说明

由于Tauri不支持跨平台编译，每个平台的安装包需要在对应的操作系统上构建：

- Windows安装包需要在Windows上构建
- macOS安装包需要在macOS上构建
- Linux安装包需要在Linux上构建

通常，macOS是项目构建中的瓶颈，因为它要求必须在macOS系统上编译。此仓库解决了这个问题，允许团队成员在各自平台上构建，然后将结果上传到这里进行集中分发。

## 如何上传新版本

1. 在相应的操作系统上构建应用程序
2. 将构建好的安装包放入对应平台的目录中
3. 提交并推送更改到此仓库
4. 在GitHub Releases中创建新版本发布

## 关联项目

- [主代码仓库](https://github.com/langkeyo/tauri-daily-helper) - 日报助手的源代码仓库