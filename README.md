# MSLX Plugin Templates (dotnet new 模板仓库)

本仓库是 [MSLX](https://github.com/MSLTeam/MSLX) 的官方 `dotnet new` 插件脚手架模板包。

---

## 🚀 安装模板

### 从 NuGet 安装（推荐）
```bash
dotnet new install MSLX.Plugin.Templates
```

### 从本地仓库安装（开发与测试）
```bash
dotnet new install /path/to/mslx-plugin-templates
```

---

## 📦 创建插件项目

```bash
dotnet new mslx-plugin -n MSLX.Plugin.MyAwesome \
  --plugin-id mslx-plugin-awesome \
  --plugin-name "我的超棒插件" \
  --plugin-author "YourName"
```

### 可用参数

| 参数 | 简写 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| `-n, --name` | `-n` | 项目/程序集名称 (PascalCase，如 `MSLX.Plugin.MyAwesome`) | 当前目录名 |
| `--plugin-id` | `-pi` | 插件唯一标识符 (规范：`mslx-plugin-xxx`) | `mslx-plugin-custom` |
| `--plugin-name` | `-pn` | 插件中文/显示名称 | `MSLX 自定义插件` |
| `--plugin-author`| `-pa` | 插件开发者/作者名称 | `developer` |
| `--description` | `-de` | 插件描述信息 | `基于 MSLX.SDK 构建的插件项目` |

---

## 🛠️ 打包模板 NuGet 包（仓库维护者）

```bash
dotnet pack
```

构建生成的 `.nupkg` 文件位于 `nupkg/` 目录。
