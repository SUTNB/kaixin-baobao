# 开心宝宝 · 安装包

macOS 桌面宠物「开心宝宝」的安装包下载页。**这里只放安装包，源码不公开。**

## 下载

| 你的 Mac | 文件 |
| --- | --- |
| Apple 芯片（M1/M2/M3/M4） | [KaixinBaobao-0.3.1-arm64.dmg](https://github.com/SUTNB/kaixin-baobao/releases/download/v0.3.1/KaixinBaobao-0.3.1-arm64.dmg) |
| Intel 芯片 | [KaixinBaobao-0.3.1-x64.dmg](https://github.com/SUTNB/kaixin-baobao/releases/download/v0.3.1/KaixinBaobao-0.3.1-x64.dmg) |

### 建议用终端命令下载（重要）

用浏览器 / 微信 / 网盘下载，macOS 会给文件打上「隔离标记」，第一次打开会被系统拦一次。用 `curl` 下载则不会：

```bash
curl -L -o ~/Downloads/KaixinBaobao.dmg \
  "https://github.com/SUTNB/kaixin-baobao/releases/download/v0.3.1/KaixinBaobao-0.3.1-arm64.dmg"
```

（Intel 机器把文件名换成 `KaixinBaobao-0.3.1-x64.dmg`）

## 安装

1. 双击下载好的 DMG，把 **KaixinBaobao.app** 拖进「应用程序」；
2. 直接双击打开即可。

## 如果被系统拦了

说明这个文件是浏览器/微信下载的（带了隔离标记）。两个办法：

- **图形界面**：点弹窗里的「完成」（**不要点「移到废纸篓」**）→ 打开「系统设置 → 隐私与安全性」→ 找到「已阻止 KaixinBaobao…」→ 点「**仍要打开**」→ 输一次密码 → 再双击 App。
- **终端一条命令**：

```bash
xattr -dr com.apple.quarantine /Applications/KaixinBaobao.app
```

## 说明

- 本 App 只做了 ad-hoc 签名、**未做 Apple 公证**，所以从网络下载后首次打开可能需要放行一次；
- 包内只包含卡通素材。
