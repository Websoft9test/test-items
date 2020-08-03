
# Test 自动化安装与部署

[English](/README.md) | [简体中文](/README-zh.md)  

本项目是由 [Websoft9](https://www.websoft9.com) 研发的 [Test](https://test.io/) 自动化安装程序，开发语言是 Ansible。使用本项目，只需要用户在 Linux 上运行一条命令，即可自动化安装 Test，并预配置必要项，让原本复杂的安装和与配置过程变得没有任何技术门槛。

## 配置要求

安装本项目，确保符合如下的条件：

| 条件       | 详情       | 备注  |
| ------------ | ------------ | ----- |
| 操作系统       | CentOS7.x, Ubuntu18.04, Amazon Linux2       |  可选  |
| 公有云| AWS, Azure, 阿里云, 华为云, 腾讯云 | 可选 |
| 私有云|  KVM, VMware, VirtualBox, OpenStack | 可选 |
| 服务器配置 | 最低1核1G，安装时所需的带宽不低于10M |  建议采用按量100M带宽 |

更多请见 [官方 System requirement](https://www.test.com/download.html)

## 组件

包含的核心组件为：可选 Test2.8.24/3.0.7/3.2.13/4.0.14/5.0.7/stable 多个版本

更多请见 [参数表](/docs/zh/stack-components.md)

## 本项目安装的是 Test 最新版吗？

本项目通过[Test 官方仓库源](https://packagecloud.io/test/test-server/install)安装，每次安装均可保证为最新版本。

版本号，请通过[官方下载](https://www.test.com/download.html)页面查看  

我们会定期检查版本准确性，并测试此项目，以保证用户可以顺利安装所需的Test版本。  

## 安装指南

以 root 用户登录 Linux，运行下面的**一键自动化安装命令**即可启动自动化部署。若没有 root 用户，请以其他用户登录 Linux 后运行 `sudo su -` 命令提升为 root 权限，然后再运行下面的脚本。

```
wget -N https://raw.githubusercontent.com/Websoft9/ansible-linux/master/scripts/install.sh; bash install.sh -r test
```

脚本后启动，就开始了自动化安装，必要时需要用户做出交互式选择，然后耐心等待直至安装成功。

**安装中的注意事项：**  

1. 操作不慎或网络发生变化，可能会导致SSH连接被中断，安装就会失败，此时请重新安装
2. 安装缓慢、停滞不前或无故中断，主要是网络不通（或网速太慢）导致的下载问题，此时请重新安装

多种原因导致无法顺利安装，请使用我们在公有云上发布的 [Test 镜像](https://apps.websoft9.com/test) 的部署方式


## 文档

文档链接：https://support.websoft9.com/docs/test/zh

## License

本项目是开源项目，采用 LGPL3.0 开源协议。补充条款：不允许在公有云的云市场上售卖通过本项目安装后直接或间接制作的镜像。

## FAQ

- 命令脚本部署与镜像部署有什么区别？请参考：[镜像部署-vs-脚本部署](https://support.websoft9.com/docs/faq/zh/bz-product.html#镜像部署-vs-脚本部署)
- 本项目支持在 Ansible Tower 上运行吗？支持
