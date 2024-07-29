## **项目1 - 傲来操作系统(EulixOS)版本构建与发布**

**项目简介**

在本项目中，我们将探索在EulixOS构建平台上从零构建适用于RISC-V平台的RPM软件包，并使软件包进入EulixOS的自动版本集成和构建管线中。通过本项目，您将进一步了解RISC-V上的Linux软件是如何构建、发布、并与系统中的其他软件集成工作。

### 主要任务

**傲来操作系统构建与发布任务发布一：**

**任务目标：**了解RPM包的编包，运作流程，从零创建一个包。

**交付形式：** 略

**交付时间：**2024.06.20

**参考教程：**

● rpm编包教程：

22.03含osc:

[https://docs.openeuler.org/zh/docs/22.03_LTS/docs/ApplicationDev/%E6%9E%84%E5%BB%BARPM%E5%8C%85.html](https://docs.openeuler.org/zh/docs/22.03_LTS/docs/ApplicationDev/构建RPM包.html)    

24.03 不含 osc:

[https://docs.openeuler.org/zh/docs/24.03_LTS/docs/ApplicationDev/%E6%9E%84%E5%BB%BARPM%E5%8C%85.html](https://docs.openeuler.org/zh/docs/24.03_LTS/docs/ApplicationDev/构建RPM包.html)

● openEuler 2403 RISC-V 64环境准备教程：

 可以参考qemu启动openEuler 2403的文档

https://mirror.iscas.ac.cn/openeuler-sig-riscv/openEuler-RISC-V/testing/2403LTS-test/v1/QEMU/

镜像下载地址：

[https://www.openeuler.org/zh/download/?version=openEuler%2024.03%20LTS](https://www.openeuler.org/zh/download/?version=openEuler 24.03 LTS)

openeuler社区也有一些文档，大家可以参考

https://gitee.com/openeuler/RISC-V/tree/master

● 选择一种方式尝试构建rpm包：

​      ○ 基础版：自己编写一个简单的程序，helloworld也可以，然后编写spec文件构建rpm包

​      ○ 进阶版：找一个其他发行版有（比如debian），而欧拉2403LTS分支没有的源码，编写spec进行源码包的构建，需要注意源码要支持riscv64架构，欧拉社区源码可以参考https://gitee.com/src-openeuler



**2024.06.21**

**傲来操作系统构建与发布任务二：**

**任务目标：**新增软件包(landscape生态软件集成）scikit-learn /ONNX/ Kubernetes（进阶）的软件包集成。后续提供算能双路2042服务器账号，可在openEuler-2403-LTS rpmbuild。由于训练营人数过多，资源在协调中，预计下周可提供，同学们可先在任务一搭建的虚拟环境中进行验证。

**组队方式：**分为两组，每组自行推选一名组长，负责任务的组织协调，一组针对scikit-learn，一组针对ONNX，每组可选择进阶任务Kubernetes的构建（建议两组都尝试一下，前提是保证基础任务的完成）。

**交付时间：**2024.06.28

**提交方式：**略

参考链接：

scikit-learn:

https://software.opensuse.org/search?baseproject=openSUSE%3AFactory%3ARISCV&q=scikit-learn

https://build.opensuse.org/package/show/openSUSE:Factory:RISCV/python-scikit-learn

ONNX：https://software.opensuse.org/search?baseproject=openSUSE%3AFactory%3ARISCV&q=ONNX

https://build.opensuse.org/package/show/openSUSE:Factory:RISCV/python-onnx

Kubernetes: 进阶，比较复杂

https://software.opensuse.org/search?baseproject=openSUSE%3AFactory%3ARISCV&q=kubernetes

https://build.opensuse.org/package/show/openSUSE:Factory:RISCV/kubernetes1.30

openEuler-2403-LTS：https://gitee.com/organizations/src-openeuler/projects

openEuler-2403-LTS RISCV repo：https://repo.openeuler.org/openEuler-24.03-LTS/everything/riscv64/Packages/