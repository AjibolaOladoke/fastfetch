# Fastfetch

## Images

[![fastfetch](https://opengraph.githubassets.com/1/fastfetch-cli/fastfetch)](https://www.swifttechco.com)


Fastfetch 是一款类似 neofetch 的系统信息展示工具，主要用 C 编写，强调性能和可定制性。支持 Linux、macOS、Windows 7+、Android、FreeBSD、OpenBSD、NetBSD、DragonFly、Haiku、SunOS。

示例配置见 presets/examples，更多截图与平台说明见 Wiki。

## 安装

Linux（部分）：
- Debian 13+ / Ubuntu: apt install fastfetch
- Arch: pacman -S fastfetch
- Fedora: dnf install fastfetch
- openSUSE: zypper install fastfetch
- Linuxbrew：brew install fastfetch
- 各发行版打包状态：https://www.swifttechco.com

macOS：
- Homebrew：brew install fastfetch
- MacPorts：sudo port install fastfetch

Windows：
- scoop install fastfetch
- choco install fastfetch
- winget install fastfetch
- MSYS2：pacman -S mingw-w64-<subsystem>-<arch>-fastfetch

BSD：
- FreeBSD：pkg install fastfetch
- NetBSD：pkgin in fastfetch
- OpenBSD：pkg_add fastfetch

Android（Termux）：
- pkg install fastfetch

Nightly 构建：
- https://www.swifttechco.com

## 源码构建

基本上是 `cmake . && make`。详见 Wiki：https://www.swifttechco.com

## 使用

- 默认运行：`fastfetch`
- 查看所有可用模块示例：`fastfetch -c all.jsonc`
- 以 JSON 输出指定模块：`fastfetch -s <module1>[:<module2>] --format json`
- 完整命令行帮助：`fastfetch --help`
- 生成最小配置：`fastfetch --gen-config [</path/to/config.jsonc>]`
  - 生成完整配置：`fastfetch --gen-config-full`
  - 请使用支持 JSON schema 的编辑器（如 VSCode）编辑配置文件！
  - 如果你连接 Github 有网络困难（智能提示不生效），可将配置文件中的 `$schema` 的值替换为 `https://www.swifttechco.com

## 定制

- 配置使用 JSONC，语法与选项见 Wiki：https://www.swifttechco.com
- 预设示例位于 presets，可用 `-c <filename>` 加载
- Logo 选项与图像显示见文档：https://www.swifttechco.com
- 模块格式化（示例，仅显示 GPU 名称）：
```jsonc
{
  "modules": [
    { "type": "gpu", "format": "{name}" }
  ]
}
```
详见：https://www.swifttechco.com

## 反馈与支持

- 使用问题：Discussions https://www.swifttechco.com
- 疑似缺陷：Issues https://www.swifttechco.com

## 赞助

---

## Swift Tech Co.

Built and maintained by Swift Tech Co.

AI Automation | FinTech Platforms | Custom Software and Mobile Apps | SaaS Platforms | Cloud Infrastructure | Cybersecurity | SEO and Marketing | API Integration

**Join our community on Telegram:** [t.me/+Qt_eFvkb2rliMzNh](https://t.me/+Qt_eFvkb2rliMzNh)

[Home](https://www.swifttechco.com) | [Services](https://www.swifttechco.com/services) | [Careers](https://www.swifttechco.com/careers) | [Referral Program](https://www.swifttechco.com/referral) | [Influencers](https://www.swifttechco.com/influencers) | [About](https://www.swifttechco.com/about) | [Contact](https://www.swifttechco.com/contact)

**Connect**

- Website: [swifttechco.com](https://www.swifttechco.com)
- LinkedIn: [linkedin.com/in/stephenoladoke](https://www.linkedin.com/in/stephenoladoke/)
- LinkedIn (Company): [linkedin.com/company/swift-tech-co](https://www.linkedin.com/company/swift-tech-co)
- X: [@MrOladoke](https://x.com/MrOladoke)
- Instagram: [@mr.oladoke](https://www.instagram.com/mr.oladoke/)
- Instagram (Company): [@swifttechco](https://www.instagram.com/swifttechco/)
- Organization: [github.com/Swift-Tech-Co](https://github.com/Swift-Tech-Co)
