Build from source
=================

准备工作
-------

目前 Ubuntu 18.04 / Debian 9 和 Fedora 27 等比较新的 Linux 发行版本都已经加入了 TPM 2.0 软件栈开发工具

这里以 Ubuntu 18.04 系统为例子, 介绍如何基于 Intel 开源的 TPM 2.0 软件栈进行第三方应用的开发, 运行以下两条命令:

```
sudo apt-get update
sudo apt-get install libsapi-dev libsapi-utils
```

安装 Intel 提供的 TPM 2.0 软件栈. 其中:
- 软件包 libsapi-utils 包括可执行文件 `/usr/sbin/resourcemgr` 即 Intel TPM 2.0 资源管理器
- 软件包 libsapi-dev 包括 C 头文件和动态链接库, 将被分别安装到 `/usr/include/sapi /usr/include/tcti 和 /usr/lib/{CPU架构}-linux-gnu` 目录中去

安装微软 Simulator.exe 或 IBM software TPM simulator
---------------------------------------------------
参照
https://github.com/tpm2-software/tpm2-tss/blob/2.0.1/README.md#simulator
的 README 自述文档, 安装 Windows 或 Linux 版本的模拟器
