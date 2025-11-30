# Augment-Code-Free

**中文** | [English](README_EN.md)

[![GitHub downloads](https://img.shields.io/github/downloads/vagmr/Augment-Code-free/total)](https://github.com/vagmr/Augment-Code-free/releases)

Augment-Code-Free 是一个用于清理 AugmentCode插件 相关数据的简易Gui工具

- **自动扫描** - 一键检测系统中已安装的所有支持IDE
- **跨平台支持** - Windows、macOS、Linux 全平台兼容
- **动态适配** - 根据选择的IDE类型自动调整可用操作

## 界面预览

<div align="center">

### 主界面
![主界面](docs/ui2.png)

### 操作界面
![操作界面](docs/ui.png)

</div>

## 功能特性

- 🖥️ **现代化 GUI 界面**
  - 基于 webview 的桌面应用程序
  - 直观的界面设计
  - 实时操作反馈

- 🔍 **智能 IDE 检测**
  - 自动扫描系统中已安装的IDE
  - 支持 VSCode 系列和 JetBrains 系列
  - 跨平台兼容（Windows、macOS、Linux）
  - 动态操作界面适配

- 💙 **VSCode 系列支持(vscode，vscodium,cursor等)**
  - 重置设备 ID 和机器 ID（Telemetry）
  - 清理 SQLite 数据库中的特定记录
  - 清理工作区存储文件
  - 自动备份原始数据

- 🧠 **JetBrains 系列支持(idea,pycharm,goland等)**
  - 重置 PermanentDeviceId 和 PermanentUserId
  - 自动文件锁定防止重新生成
  - 跨平台文件权限管理
  - 支持所有主流 JetBrains IDE

- 🛡️ **安全特性**
  - 操作前自动备份重要文件
  - 文件锁定机制防止意外修改
  - 详细的操作日志和结果反馈


## 安装说明

### 方式一：直接下载可执行文件（windows 推荐）

1. 从 [Releases](https://github.com/vagmr/Augment-free/releases) 页面下载最新版本
2. 解压并运行 `AugmentFree_latest.exe`

### 方式二：从源码运行

1. 确保你的系统已安装合适的python版本
2. 克隆此仓库到本地：
   ```bash
   git clone https://github.com/vagmr/Augment-free.git
   cd Augment-free
   ```
3. 安装依赖：
   ```bash
   # 使用 uv（推荐）
   uv sync

   # 或使用 pip
   pip install -e .
   ```

## 使用方法

### 使用可执行文件

1. **Augment插件退出原有账号**
2. **完全退出选择的编辑器**
3. **运行应用程序**：
   - 双击 `AugmentFree_latest.exe`
   - 或在命令行中运行：`./AugmentFree_latest.exe`
4. **在 GUI 界面中选择需要的操作**
5. **重新启动选择的编辑器**
6. **在 Augment 插件中使用新的邮箱进行登录**

### 从源码运行

1. **Augment插件退出原有账号**
2. **完全退出选择的编辑器**
3. **运行应用程序**：
   ```bash
   # 使用 run.py 脚本（推荐）
   python run.py

   # 或直接运行模块
   python -m augment_free.main
   ```
4. **在 GUI 界面中选择需要的操作**
5. **重新启动选择的编辑器**
6. **在 Augment 插件中使用新的邮箱进行登录**



### 开发环境设置

1. Fork 此仓库
2. 克隆你的fork：
   ```bash
   git clone https://github.com/你的github用户名/Augment-free.git
   ```
3. 安装开发依赖：
   ```bash
   uv sync --dev
   ```
4. 进行修改

## ⚠️ 免责声明

**使用风险自负：** 本工具仅供学习和研究目的使用，使用者需自行承担使用风险。

**数据安全：** 使用前请确保重要数据已备份，作者不对任何数据丢失负责。

**合规使用：** 请遵守相关软件的使用条款和当地法律法规。

**无担保：** 本软件按"现状"提供，不提供任何明示或暗示的担保。

**商业使用：** 所有商业售卖行为均与本人无关。

## 许可证

此项目采用 MIT 许可证。详见 [LICENSE](LICENSE) 文件。
