## 【官方加强了检测机制，本方法已不适用，请关注后续更新】

# Cursor 设备标识生成器

一个安全、简便、快捷的 Cursor Pro Trial 设备标识重置工具。

## 功能特点

- 🔒 安全可靠：纯前端生成，无需后端服务
- 🚀 快速便捷：一键生成新的设备标识
- 💻 跨平台支持：Windows、macOS 和 Linux

## 使用步骤

1. 退出cursor的登录账号，确保 Cursor 完全关闭（包括后台进程），一般关闭Cursor就可以了。
2. 打开工具页面，点击"重新生成 ID"按钮。页面地址在[这里](https://cursor-id.duu.men/),或看简介链接
3. 根据您的操作系统，找到并打开对应的配置文件：
   - Windows（win键+R，输入）: `%APPDATA%\Cursor\User\globalStorage\storage.json`
   - macOS: `~/Library/Application Support/Cursor/User/globalStorage/storage.json`
   - Linux: `~/.config/Cursor/User/globalStorage/storage.json`
4. 将生成的三个标识码复制替换到配置文件中：
   - `telemetry.macMachineId`
   - `telemetry.machineId`
   - `telemetry.devDeviceId`
5. 保存文件
6. 重新启动 Cursor 并登录
7. 确保Cursor Pro Trial（pro测试） 账号正常，就可以正常使用了。

## 快速访问配置文件

### Windows
1. 按 `Win + R` 打开运行对话框
2. 粘贴 `%APPDATA%\Cursor\User\globalStorage\storage.json`
3. 点击确定

### macOS
1. 在 Finder 中按 `Command + Shift + G`
2. 粘贴 `~/Library/Application Support/Cursor/User/globalStorage/storage.json`
3. 点击前往

### Linux
直接在终端中使用编辑器打开：
```bash
nano ~/.config/Cursor/User/globalStorage/storage.json
或
vim ~/.config/Cursor/User/globalStorage/storage.json
```

## 注意事项

- ⚠️ 使用前请确保 Cursor 完全关闭
- 💾 建议在修改前备份原配置文件
- 🔄 如果修改后无效，请检查 Cursor 是否还在后台运行。

## 免责声明

本工具仅供学习和研究使用。使用本工具产生的任何问题和风险由使用者自行承担。cursor 是一个不错的编辑器，条件允许，请购买支持。
