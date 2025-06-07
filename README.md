根据陈天老师的训练营创建的模板,对模板进行了较新版本的更新

## 使用模板时记得修改将TODO的地方进行修改
## 模板要求

### VSCode 插件（可选）

- crates: Rust 包管理
- Even Better TOML: TOML 文件支持
- Better Comments: 优化注释显示
- Error Lens: 错误提示优化
- GitLens: Git 增强
- Github Copilot: 代码提示
- indent-rainbow: 缩进显示优化
- Prettier - Code formatter: 代码格式化
- REST client: REST API 调试
- rust-analyzer: Rust 语言支持
- Rust Test lens: Rust 测试支持
- Rust Test Explorer: Rust 测试概览
- todo Highlight: todo 高亮
- vscode-icons: 图标优化
- YAML: YAML 文件支持

### 安装 cargo generate

用于生成项目模板。

```bash
cargo install cargo-generate
```

```bash
cargo generate github_name/repo
```
[text]["https://github.com/cargo-generate/cargo-generate"]

### 安装 pre-commit

代码检查。

```bash
pipx install pre-commit
```

安装成功后运行 `pre-commit install`可在当前项目安装pre-commit 。

用pre-commit测试的方法
```bash
pre-commit run --all-files
```
[text][pre-commit.com]

### 安装 Cargo deny

用于检查依赖的安全性。

```bash
cargo install --locked cargo-deny
```

插件测试方法(一般来说pre-commit就包含了它的方法)
```bash
cargo deny check
```

### 安装 typos

拼写检查。

```bash
cargo install typos-cli
```

### 安装 git cliff

生成 changelog。

```bash
cargo install git-cliff
```

它会在如下情况生成changelog
```bash
git tag -a v0.*.*
```

### 安装 cargo nextest

Rust 增强测试工具。

```bash
cargo install cargo-nextest --locked
```
