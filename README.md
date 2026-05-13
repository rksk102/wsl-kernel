# WSL2 内核自动编译

自动从 [microsoft/WSL2-Linux-Kernel](https://github.com/microsoft/WSL2-Linux-Kernel) 获取最新源码，交叉编译 x64 和 ARM64 架构的 WSL2 内核镜像，并发布到 [GitHub Releases](https://github.com/rksk102/wsl-kernel/releases)。

## 使用方式

从 Releases 页面下载对应架构的 `bzImage` 文件，替换 Windows 中的 WSL2 内核。

## 触发方式

- **定时触发**: 每 2 天自动检查上游是否有新版本
- **手动触发**: 在 Actions 页面使用 `workflow_dispatch`，可指定特定标签