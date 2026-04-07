# Homebrew Tap

个人 Homebrew Tap 仓库，包含以下实用工具：

## 可用工具

### [jenkins-job-cli](https://github.com/jeffzhangc/jenkins-job-cli)

Jenkins CLI 工具，用于程序化管理 Jenkins 任务。

**功能特性：**
- 程序化管理 Jenkins jobs
- 支持 shell 补全（bash/zsh/fish）
- 跨平台支持（macOS Intel/Apple Silicon, Linux x86_64/ARM64）

**安装：**
```bash
brew install --cask jeffzhangc/tap/jenkins-job-cli
```

**使用：**
```bash
jj --help
```

**启用 Shell 补全：**
```bash
# Zsh
echo 'source <(jj completion zsh)' >>~/.zshrc

# Bash
echo 'source <(jj completion bash)' >>~/.bashrc
```

**卸载：**
```bash
brew uninstall --cask jeffzhangc/tap/jenkins-job-cli
```

---

### [sshpky](https://github.com/jeffzhangc/go-sshpky)

SSH 工具，简化 SSH 密钥管理和连接操作。

**功能特性：**
- 简化 SSH 密钥管理
- 支持 shell 补全（bash/zsh/fish）
- 跨平台支持（macOS Intel/Apple Silicon, Linux x86_64/ARM64）

**安装：**
```bash
brew install --cask jeffzhangc/tap/sshpky
```

**使用：**
```bash
sshpky help
```

**卸载：**
```bash
brew uninstall --cask jeffzhangc/tap/sshpky
```

> **注意：** 配置文件存储在 `~/.sshpky`。如需完全卸载所有配置数据，可删除此目录。

---

## 使用方法

### 添加 Tap 仓库

```bash
brew tap jeffzhangc/tap https://github.com/jeffzhangc/tap
```

### 查看可用工具

```bash
brew search jeffzhangc/tap
```

### 更新工具

```bash
brew upgrade --cask jenkins-job-cli
brew upgrade --cask sshpky
```

## 系统要求

- macOS (Intel 或 Apple Silicon)
- Linux (x86_64 或 ARM64)
- Homebrew 已安装

## 版本说明

Cask 文件由 [GoReleaser](https://goreleaser.com/) 自动生成，每次发布新版本时自动更新。

## 许可证

[MIT License](LICENSE)

## 问题反馈

如有问题或建议，请在对应的 GitHub 仓库提交 Issue：
- [jenkins-job-cli Issues](https://github.com/jeffzhangc/jenkins-job-cli/issues)
- [sshpky Issues](https://github.com/jeffzhangc/go-sshpky/issues)
