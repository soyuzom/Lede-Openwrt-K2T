# Actions自动编译OpenWrt固件

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Forks&logo=github)

使用GitHub Actions构建OpenWrt

[【详细教程】](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

## 使用方法

- 点击 [Use this template](https://github.com/P3TERX/Actions-OpenWrt/generate) 按钮以创建新的存储库。
- 使用 [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) 生成的`.config`文件. ( 您可以通过工作流文件中的环境变量来更改它。 )
- 将 `.config` 文件推送到GitHub存储库，构建会自动开始。进度可以在`Actions`页面上查看。
- 构建完成后，单击`Actions`页面右侧`Artifacts`栏内的文件直接下载。

### 提示

创建`.config`文件并构建OpenWrt固件可能需要很长时间。 因此，在创建存储库以构建自己的固件之前，您可以通过 [在GitHub里搜索 `Actions-Openwrt` ](https://github.com/search?q=Actions-openwrt)，检查是否已经建立了其他满足您需要的固件。

将您所构建固件的一些元信息（例如固件体系结构和已安装的软件包）添加到存储库简介中，这将节省其他人的时间。


### 固件说明

- 已测试固件： [https://idoog.lanzous.com/b0kd0oeb](https://idoog.lanzous.com/b0kd0oeb)

- 未测试最新编译：[自动编译版](https://github.com/soyuzom/Lede-Openwrt-K2T/actions)

- #### K2T默认登陆IP 192.168.10.1, 密码 password
- #### K2 默认登陆IP 192.168.20.1, 密码 password

- [Lean's OpenWrt源码仓库](https://github.com/coolsnowwolf/lede) 


## 感谢

- [Microsoft](https://www.microsoft.com)
- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub](https://github.com)
- [GitHub Actions](https://github.com/features/actions)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cisco](https://www.cisco.com/)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)

## 许可

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE) © P3TERX
