# 【已关闭更新】
### 固件说明


- 最新编译：[【自动编译版】](https://github.com/soyuzom/Lede-Openwrt-K2T/actions)  [【Releases】](https://github.com/soyuzom/Lede-Openwrt-K2T/releases)  

- **K2T默认登陆IP 192.168.10.1, 密码 password**
- **K2 默认登陆IP 192.168.2.1, 密码 password**

 K2  为：**openwrt-ramips-mt7620-phicomm_psg1218a-xxx**

K2T 为：**openwrt-ath79-generic-phicomm_k2t-xxx**

- 固件 版本号同  [Lean's OpenWrt源码仓库](https://github.com/coolsnowwolf/lede) 

#### 注 K2：因为K2内存比较小，最新版固件塞不进SSR，只塞进[Turbo ACC  FLOW转发加速]、[释放内存]、[中继配置]
------------------------------------------------------


# Actions自动编译OpenWrt固件

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Forks&logo=github)

使用GitHub Actions构建OpenWrt

[【详细教程】](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

## 使用方式

- 点击 [Use this template](https://github.com/P3TERX/Actions-OpenWrt/generate) 按钮创建新的库。
- 使用 [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) 源码生成`.config`文件 (您可以通过工作流文件中的环境变量来更改它。看*提示2*)
- 将 `.config` 文件推送到 GitHub 库。
- 在自动编译`Actions`页面选择 `Build OpenWrt`
- 点击 `Run workflow` 按钮。
- 将您所构建固件的一些元信息（例如固件体系结构和已安装的软件包）添加到存储库简介中，这将节省其他人的时间。

## 提示1

- 创建`.config`文件并构建OpenWrt固件可能需要很长时间。 因此，在创建存储库以构建自己的固件之前，您可以通过 [在GitHub里搜索 `Actions-Openwrt` ](https://github.com/search?q=Actions-openwrt)，检查是否已经建立了其他满足您需要的固件。
- 将您所构建固件的一些元信息（例如固件体系结构和已安装的软件包）添加到存储库简介中，这将节省其他人的时间。

## 提示2

- 在Run Workflow时把SSH connection to Actions的值改为true（或者也可以不修改，而是通过 webhook 方式发送带有ssh触发关键词的请求。）
- 在触发工作流程后，在 Actions 日志页面等待执行到SSH connection to Actions步骤，会出现类似下面的信息：

  **To connect to this session copy-n-paste the following into a terminal or browser:**
  
  **ssh Y26QeagDtsPXp2mT6me5cnMRd@nyc1.tmate.io**
  
  **https://tmate.io/t/Y26QeagDtsPXp2mT6me5cnMRd**
  
- 复制 SSH 连接命令粘贴到终端内执行，或者复制链接在浏览器中打开使用网页终端。（网页终端可能会遇到黑屏的情况，按 Ctrl+C 即可）

  **cd openwrt && make menuconfig**

- 完成后按Ctrl+D组合键或执行exit命令退出，后续编译工作将自动进行。
- 固件目录下有个config.seed文件，如果你需要再次编译可以使用它。

------------------------------------------------------

## 致谢

- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [ActionsRML/delete-workflow-runs](https://github.com/ActionsRML/delete-workflow-runs)
- [dev-drprasad/delete-older-releases](https://github.com/dev-drprasad/delete-older-releases)
- [peter-evans/repository-dispatch](https://github.com/peter-evans/repository-dispatch)

## License

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/main/LICENSE) © [**P3TERX**](https://p3terx.com)
