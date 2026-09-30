<p align="center"><img src="docs/assets/logo-small.png" alt="MarkText" width="100" height="100"></p>

<h1 align="center">MarkText 中文版</h1>

<div align="center">
  <strong>:high_brightness: 下一代 Markdown 编辑器（简体中文发行版） :crescent_moon:</strong><br>
  一款简洁优雅的开源 Markdown 编辑器，专注速度与易用性。<br>
  <sub>支持 Linux、macOS 和 Windows。</sub>
</div>

<br>

> **说明**  
> 本仓库是 [MarkText](https://github.com/marktext/marktext) 的**简体中文增强分支**，默认界面为中文，并内置语言包插件扩展能力。  
> 原始项目以 **MIT** 协议开源，版权归原作者所有；本分支保留全部版权声明与协议正文，见 [LICENSE](LICENSE)。

<br>

<div align="center">
  <a href="LICENSE">
    <img src="https://img.shields.io/github/license/marktext/marktext.svg" alt="LICENSE">
  </a>
  <a href="https://github.com/marktext/marktext">
    <img src="https://img.shields.io/badge/upstream-marktext%2Fmarktext-blue" alt="upstream">
  </a>
</div>

<div align="center">
  <h3>
    <a href="https://github.com/marktext/marktext">上游 MarkText</a>
    <span> | </span>
    <a href="#功能特性">功能特性</a>
    <span> | </span>
    <a href="#下载与安装">下载安装</a>
    <span> | </span>
    <a href="#语言包插件">语言包</a>
  </h3>
</div>

---

## 与原版的差异

| 项 | 说明 |
| --- | --- |
| 默认语言 | 简体中文（可在偏好设置切换） |
| 界面文案 | 菜单、对话框、提示已完整汉化 |
| 语言包插件 | 支持热插拔语言包，丢 JSON 即可扩展新语言 |
| 配置兼容 | 启动时自动修复非法配置枚举值，避免崩溃 |
| 稳定性 | 缺少原生模块时可降级启动 |

## 界面截图

![](docs/assets/marktext.png?raw=true)

## 功能特性

- 实时预览（所见即所得），界面简洁，专注写作。
- 支持 [CommonMark 规范](https://spec.commonmark.org)、[GitHub Flavored Markdown 规范](https://github.github.com/gfm/)，并选择性支持 [Pandoc markdown](https://pandoc.org/MANUAL.html#pandocs-markdown)。
- Markdown 扩展：数学公式（KaTeX）、前置元数据（Front Matter）、表情符号等。
- 支持段落与行内样式快捷键，提升写作效率。
- 可导出 **HTML** 与 **PDF**。
- 多种[主题](https://marktext.me/docs/themes)：**Cadmium Light**、**Material Dark** 等。
- 多种编辑模式：**源码模式**、**打字机模式**、**专注模式**。
- 支持直接从剪贴板粘贴图片。
- **默认界面语言为简体中文**。

## 下载与安装

Windows 用户可自行编译安装包：

```bash
git clone https://github.com/hujinlong989/marktext.git
cd marktext
pnpm install
pnpm run build:win
# 安装包位于 dist/ 目录
```

编译需要 [Visual Studio Build Tools（C++ 桌面开发）](https://visualstudio.microsoft.com/visual-cpp-build-tools/)。

## 语言包插件

支持热插拔语言包：把 JSON 或文件夹丢进 `%APPDATA%\marktext\lang-packs\`，重启后在「偏好设置 → 通用 → 语言」中选用。

- 详细说明：[docs/i18n/LANGUAGE_PACKS.md](docs/i18n/LANGUAGE_PACKS.md)
- 示例语言包：[docs/i18n/examples/lang-packs/](docs/i18n/examples/lang-packs/)

## 开发

```bash
pnpm install
pnpm run dev        # 开发模式
pnpm run build      # 构建
pnpm run test       # 测试
pnpm run lint       # 代码检查
```

更多开发文档见上游 [Developer Documentation](https://marktext.me/docs/dev/overview)。

## 贡献

欢迎提交 Issue 与 Pull Request 到本仓库。  
若要向**上游**贡献，请先阅读 [MarkText 贡献指南](https://github.com/marktext/marktext/blob/develop/.github/CONTRIBUTING.md)。

## 许可证与版权

本项目基于 **MIT License** 开源。

```text
MIT License

Copyright (c) 2017-present Luo Ran
Copyright (c) 2018-present MarkText Contributors
```

完整协议见 [LICENSE](LICENSE)。你可以自由使用、修改、分发，但须保留上述版权声明与 MIT 协议文本。

---

<p align="center">
  原始项目由 <a href="https://github.com/Jocs">Jocs</a> 与 <a href="https://github.com/marktext/marktext/graphs/contributors">MarkText 贡献者们</a> 用 ❤︎ 构建。
</p>
