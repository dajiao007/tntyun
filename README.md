<div align="center">

**🚀 TNTCloud 新手使用指南：基于 Clash Verge (v2.7.4) 的全流程路书**

欢迎找到TNTCloud 的世界！🎉
![TNTCloud 页面示意图](image/pic.webp)
👉 **TNTCloud 官网入口：** [TNTCloud 官网](https://tntyun.cc/#/register?code=CZVdpQnI)

</div>

---

 ## **一、 💡 TNTCloud 简要介绍**

 TNTCloud 是一家提供高速、稳定、安全的网络代理服务提供商。通过部署在全球的优质服务器节点，它可以帮助您突破网络限制，保护隐私，并享受流畅的国际互联网体验。

---

## **二、 💻 客户端选择**

为了连接到 TNTCloud 的节点，您需要在您的设备上安装相应的客户端软件。

| 平台 | 客户端 |
| --- | --- |
| 桌面端主力推荐（本指南重点） | **Clash Verge (v2.7.4)**。它界面美观、功能强大，支持 Windows、macOS 和 Linux 平台。 |
| Android (安卓) | 推荐使用 [Clash for Android](https://www.google.com/search?q=https://github.com/Kr328/ClashForAndroid) 🤖 或 [Surfboard](https://github.com/getsurfboard/surfboard) 🏄‍♂️。 |
| iOS (苹果手机) | 推荐在非国区 App Store 下载 **Shadowrocket**（小火箭）🚀 或 **Quantumult X**。 |
| macOS (苹果电脑) | 除 Clash Verge 外，也可选用 [ClashX Pro](https://install.appcenter.ms/users/clashx/apps/clashx-pro/distribution_groups/public) 🍎。 |

---

## **三、 🛠️ Clash Verge (v2.7.4为例) 核心配置指南**

以下步骤将引导您完成从下载到最终使用的全过程。请务必仔细阅读**核心步骤**！

<details open>
<summary><strong>1. 下载与安装（关键要素）🔑</strong></summary>

* **获取软件：** 请前往 Clash Verge 的开源发布页面（GitHub Releases）下载对应您系统的 v2.7.4 安装包（Windows 用户通常下载 .exe 结尾的文件）。  
* **安装：** 按照系统默认提示“下一步”完成安装即可。首次打开可能会有防火墙提示，请务必选择**允许访问**。

</details>

<details open>
<summary><strong>2. 在 Clash Verge 中配置订阅 (核心步骤) 🔗</strong></summary>

订阅链接是连接 TNTCloud 服务的“钥匙”。

1. **获取订阅链接：** 登录 [TNTCloud 官网](https://tntyun.cc/#/register?code=CZVdpQnI)，在用户后台首页找到“一键订阅”或“导入到 Clash”按钮，点击**复制 Clash 订阅链接**。  
2. **导入到 Clash Verge：**  
   * 打开 Clash Verge 客户端。  
   * 点击左侧导航栏的 **“配置” (Profiles)** 📂。  
   * 在顶部的输入框中，**粘贴**您刚刚复制的 TNTCloud 订阅链接。  
   * 点击右侧的 **“导入” (Import)** 按钮。  
   * 等待几秒钟，列表下方会出现一个新增的配置卡片（通常命名为 TNTCloud）。  
   * **单击该卡片**，使其背景变色或出现选中图标，代表已激活该配置。

</details>

<details open>
<summary><strong>3. 选择代理与模式 (核心步骤) 🕹️</strong></summary>

配置激活后，您需要告诉软件如何处理您的网络请求。

1. 点击左侧导航栏的 **“代理” (Proxies)** 🛡️。  
2. **选择代理模式（右上角）：**  
   * **规则 (Rule)：** **【强烈推荐】** 智能分流模式。访问国内网站直连（不走流量），访问国外网站走代理。  
   * **全局 (Global)：** 所有网络请求强制通过代理节点（适用于特定场景）。  
   * **直连 (Direct)：** 关闭代理，所有请求直接发送。  
3. **选择节点：** 在代理面板中，您会看到一个名为 PROXIES 或 节点选择 的策略组。展开它，您可以手动点击选择一个延迟较低（绿色数字小）的 TNTCloud 节点，例如“香港 01”或“日本 02”。点击右上角的闪电图标⚡️可以测试节点延迟。

</details>

<details open>
<summary><strong>4. 配置规则与分流 (进阶了解) 🧠</strong></summary>

Clash Verge 的强大之处在于其灵活的规则系统。

* 通常情况下，TNTCloud 提供的订阅中已经内置了完善的规则集（如针对广告拦截、流媒体解锁等），您保持默认的 **“规则 (Rule)”** 模式即可，无需手动干预。  
* 如果您需要自定义特定网站的走向，可以前往 **“规则” (Rules)** 界面进行查阅，或在 **“设置”** 中通过配置文件（YAML）添加自定义脚本。*（新手建议先不作修改，以免影响正常使用）*。

</details>

<details open>
<summary><strong>5. 其他重要配置 (保障最佳体验) 🚀</strong></summary>

为了让代理生效并提升使用体验，请检查以下设置：

* **开启系统代理 (System Proxy)：** 点击左侧 **“设置” (Settings)** ⚙️，在“系统设置”板块中，打开 **系统代理 (System Proxy)** 开关。此时您的浏览器就可以科学上网了！🌎

* **开启 TUN 模式 (虚拟网卡)：** 如果您发现某些桌面软件（如 Telegram、游戏客户端）无法联网，请在“设置”中开启 **TUN 模式**。这会在系统底层接管所有网络流量。首次开启可能需要授予管理员权限。  
* **开机自启：** 在“设置”中找到 **开机启动 (Start with Windows)** 并开启，避免每次重启电脑都要手动打开软件。  


</details>

---

## ** 🚀 Enjoin it **

---

> **免责声明**：本指南仅供技术交流及学习参考。请遵守当地法律法规，合理合法使用网络资源。。
>
 👉 **TNTCloud 官方入口：** [TNTCloud 官网](https://tntyun.cc/#/register?code=CZVdpQnI)
