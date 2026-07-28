# 贡献指南

非常欢迎并感谢你对 **JSON 格式化与查看工具** 的关注与贡献！无论是修复 Bug、提出新功能、改进文档，还是提交翻译，都是对项目的支持。

- 源码仓库：https://github.com/wangruofeng/json-viewer
- 在线访问：https://blog.wangruofeng007.com/json-viewer/

## 在开始之前

- 提交新功能或较大改动前，建议先在 [Issues](https://github.com/wangruofeng/json-viewer/issues) 中发起讨论，说明你的想法与方案，避免与已有工作重复或方向不一致。
- 提交 Bug 反馈时，请尽量包含：复现步骤、预期结果、实际结果、浏览器与系统版本，必要时附上可复现的 JSON 样例。

## 开发须知

本项目是一个**纯前端的单文件应用**，所有逻辑集中在 `index.html` 中：

- 原生 HTML / CSS / JavaScript，**零依赖、零构建步骤**；
- 直接用浏览器打开 `index.html` 即可调试，无需安装任何工具链；
- 所有解析与渲染均在浏览器本地完成，请保持「不引入外部依赖、不依赖后端」的设计原则。

### 本地调试

```bash
# 克隆仓库
git clone https://github.com/wangruofeng/json-viewer.git
cd json-viewer

# 直接用浏览器打开 index.html，或启动一个本地静态服务器
python3 -m http.server 8000
# 访问 http://localhost:8000/index.html
```

## 提交 Pull Request

1. Fork 本仓库，并基于 `main` 分支创建特性分支：
   ```bash
   git checkout -b feat/your-feature
   ```
2. 完成开发与自测（请在主流浏览器中验证交互效果）。
3. 保持代码风格与现有代码一致：
   - 缩进、命名、注释风格对齐 `index.html` 中已有的写法；
   - 新增注释使用简体中文。
4. 提交信息遵循 [Conventional Commits](https://www.conventionalcommits.org/) 规范（中文描述亦可），例如：
   - `feat: 新增从 URL 导入功能`
   - `fix(ui): 修复深色模式下按钮对比度`
   - `docs: 补充贡献指南`
   - `refactor: 简化树形渲染逻辑`
5. 在 PR 描述中说明改动内容、动机以及是否需要更新文档。

## 代码审查

所有提交都需要经过维护者审查。审查关注正确性、可维护性与一致性。请以开放的心态对待反馈意见；如有分歧，以项目长期可维护性为优先依据。

## 行为准则

参与本项目即代表你同意遵守 [行为准则](CODE_OF_CONDUCT.md)。请在所有交流中保持友善与尊重。

再次感谢你的贡献！
