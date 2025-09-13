# luci-app-passwall2

## 说明

本项目编译输出为 **APK 格式** 的安装包，适用于基于 Alpine Linux 的 OpenWrt 系统。

### 编译输出

- `luci-app-passwall2-*.apk` - 主应用包
- `luci-i18n-passwall2-zh-cn-*.apk` - 中文语言包

### 安装方法

```bash
# 安装主包
apk add --allow-untrusted luci-app-passwall2-*.apk

# 安装中文语言包（可选）
apk add --allow-untrusted luci-i18n-passwall2-zh-cn-*.apk
```

### 支持平台

- Qualcomm IPQ8071A 系列芯片
- ARM64 (aarch64_cortex-a53) 架构
- 基于最新 OpenWrt snapshots 构建

### 自动构建

项目配置了 GitHub Actions 自动构建，每次创建 tag 或手动触发时会自动编译并发布 APK 包。
