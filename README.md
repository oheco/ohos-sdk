# ohos-sdk（历史归档）

本仓库停止更新。官方工具与 SDK 已统一迁移到
[oheco/command-line-tools](https://github.com/oheco/command-line-tools)，当前版本为
`26.0.0.201`。五个旧组件已从当前软件目录退出，历史 Release、摘要和文件保持不变。

升级 oo 到0.11.0后，仅对已安装的旧命令包运行
`oo unlink ohos-sdk-native ohos-sdk-toolchains`，即可释放默认及版本命令入口，同时保留
全部源文件和原始收据；再 `oo install command-line-tools`。无命令的ETS/JS/previewer无需unlink。
新包不导出 Node/npm/npx/corepack，不再由oo生成SDK视图。

`oo sdk` 及视图卸载保护已删除。旧视图仍依赖精确组件文件；继续使用旧工程时保留这些版本，
显式remove/cascade/autoremove可能使其失效。Godot Editor此次暂缓迁移。
完整步骤见 [迁移说明](https://github.com/oheco/oheco/blob/main/docs/MIGRATION.md)。

以下为历史版本信息。

本仓库用于分发来自开源鸿蒙（OpenHarmony）的工具链，压缩包请前往 [Releases](https://github.com/oheco/ohos-sdk/releases) 下载。

工具链源码请前往 [OpenHarmony 官方仓库](https://gitcode.com/openharmony) 获取。

## 支持的版本

| 版本（点击下载） | 平台 | 包含组件 | 发布状态 |
| --- | --- | --- | --- |
| [26.0.0.35-Beta](https://github.com/oheco/ohos-sdk/releases/tag/26.0.0.35-Beta) | `ohos-arm64` | `ets`、`js`、`native`、`previewer`、`toolchains` | 预发布（Beta） |
