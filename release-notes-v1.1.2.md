# 烤鸭极简截图 1.1.2

## 功能

- 单击系统托盘图标打开剪贴板；关闭面板后可再次单击打开。
- 保留截图、录屏、剪贴板历史、贴图及待办。
- 月历支持右键添加、修改和删除日子名称，日子信息显示在月历下方。
- 待办通过右上角加号添加；面板初始 430×600，切栏目不自动放大。
- 便携 OCR 不包含在本版本中。

## 版本与成品

本次整理现有 1.1.2，统一程序内部版本、源码标签和公开更新通道，不另发新版本号。

- 程序文件：KaoyaScreenshot.exe。
- 产品版本：1.1.2；文件及程序集版本：1.1.2.0。
- 文件大小：25,156,096 字节。
- SHA-256：E43CF681A665CF6C7D8DADF8D25F373BC96DEEE1BDA6BF47E957643138E0214A。
- 公开下载：https://github.com/dianzihuang2/kaoya-screenshot-releases/releases/tag/v1.1.2
- 公开清单：https://github.com/dianzihuang2/kaoya-screenshot-releases/blob/main/update-v2.json
- 1.1.1 可识别本次 1.1.2 更新；同版本不重复提示更新。安装仍需用户确认。

## 构建与验证

- 包含 RECORDING 和 FEATURE_TODO；未包含 PORTABLE_OCR。
- 录屏包 SHA-256：74799EEBEC38392FA0D3770897E4D9B444FEE75108C4BBCD8E387961739F745E。
- 录屏对应源码：https://github.com/dianzihuang2/obs-kaoya/tree/ed9b3cc19f13d4adebd50a77d49114ae712f6c01
- 对应应用源码和构建材料以 KaoyaScreenshot-1.1.2-source.zip 随公开 Release 提供。
- 本地完整 /selftest、/recording-selftest、托盘、贴边、月历、截图首帧、待办持久化验证通过。
- 仅修复发布自测的反射签名和测试数据隔离；不恢复已放弃的搜索、减少动画及待办保存回滚改动。
- 未覆盖全部混合 DPI、GPU、远程桌面和长时间音画同步场景。

## 历史修订说明

旧 v1.1.2 标签曾指向 0fbb8fc，附件却包含后续托盘修复，内部版本仍为 1.1.1。本轮将标签更新到整理后的发布提交。
旧标签对象、旧附件和更新清单保存在本地 backups/github-alignment-20260913/。此后发布应先确定源码提交和内部版本，再上传同一成品并验证公开下载，最后更新清单。
