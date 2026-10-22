<div align="center">

# ColorOS 移植项目

简体中文&nbsp;&nbsp;|&nbsp;&nbsp;[English](/README_en-US.md)

</div>

## 项目简介

用于将 ColorOS / OxygenOS 移植到部分一加和 OPPO 设备的自动化工具。仓库覆盖 Android 14–17 代际，但支持情况按分支、机型和底包组合而异；这不代表每个组合都已验证。开始前请确认当前分支、设备代号和 ROM 版本。

## 目标机型

- 一加 8 系列：OnePlus 8、8 Pro、8T、9R
- 一加 9 系列：OnePlus 9、9 Pro、9RT
- OPPO Find X3、Find X3 Pro

机型列表表示项目目标范围，不等同于每个分支的完整测试矩阵。

## 历史测试记录

以下版本来自旧版项目说明，仅作历史参考，不保证适用于当前分支或所有机型：

- 底包：OnePlus 8T（ColorOS 14.0.0.600）、OnePlus 8（ColorOS IN2010 13.1.190）、OnePlus 8 Pro（ColorOS IN2020 13.1.0.190）
- 移植包：OnePlus 12（ColorOS 14.0.0.800）、OnePlus Ace 3V（ColorOS 14.0.1.621）

旧版说明曾报告人脸解锁、屏下指纹、相机、NFC 和自动亮度可用，也记录过 AOD 亮度、语音唤醒、关机充电及有线耳机问题。实际情况可能随机型、分支和 ROM 版本变化；反馈问题时请附上完整的版本信息。

## 使用方法

在 WSL、Ubuntu、Deepin 等 Linux 环境中操作：

```shell
sudo apt update
sudo apt install git -y
git clone https://github.com/toraidl/coloros_port.git
cd coloros_port
sudo ./setup.sh
sudo ./port.sh /path/to/base-rom /path/to/port-rom
```

请使用你有权获取的底包和移植包。刷机前备份重要数据，并核对目标设备、分区和刷机方式；操作不当可能导致数据丢失或设备无法启动。请勿在 Issue 中上传完整 ROM、密钥、设备序列号或其他个人数据。

## 参与维护

- [贡献指南](CONTRIBUTING.md)：提交问题和 Pull Request 时需要提供的信息。
- [维护计划](docs/MAINTENANCE_PLAN.md)：兼容性记录、发布说明和自动化检查的后续计划。

## 致谢

本项目使用了以下开源项目的部分或全部内容，感谢这些项目的开发者（排名不分先后）：

- [BypassSignCheck](https://github.com/Weverses/BypassSignCheck) by Weverses
- [contextpatch](https://github.com/ColdWindScholar/TIK) by ColdWindScholar
- [fspatch](https://github.com/affggh/fspatch) by affggh
- [gettype](https://github.com/affggh/gettype) by affggh
- [lpunpack](https://github.com/unix3dgforce/lpunpack) by unix3dgforce
- [miui_port](https://github.com/ljc-fight/miui_port) by ljc-fight
