# 烤鸭箱 1.1.3

## 更新功能

1. **待办与日程体验增强**：
   - 点击待办顶栏右上角加号添加事项时，支持自由选择事项归属日期（带月历选择器与动态标题联动）；
   - 截止提醒时间与所选目标日期智能合成；
   - 编辑已有事项时支持修改所属日期（改期），并自动移动事项与对齐提醒；
   - 全局每日事项支持设定时间提醒与提前提醒通知，字号适度加大便于阅读浏览。

2. **日历导航操作优化**：
   - 顶部翻页左箭头（‹）与右箭头（›）按钮字体加大为 15pt Bold，列宽增至 38px 并增加浅灰悬停反馈；
   - 双击月份导航栏空白处或月份文本时，自动跳转回本月今天并高亮选中，多日总览视图联动平滑滚动。

3. **剪贴板贴边与缩放体验升级（方案A）**：
   - 贴边收起后呈现为小图标，取消鼠标悬停展开，改为单击展开；
   - 支持按住鼠标左键拖动小图标在屏幕边缘自由移动和吸附；
   - 底部两角扩大感应判定范围至 20px，支持底部两角与底边等比例缩放；
   - 采用方案A主线程瘦身架构：拖拽缩放期间置空不规则区域、跳过昂贵的 Win32 SetWindowRgn 频繁重置，并推迟剪贴板列表与日历多卡片的深度重排计算；
   - 配合顶层 WS_EX_COMPOSITED 离屏合成层与 Windows 11 DWM 原生硬件圆角，彻底消除边缘拖动缩放时的撕裂感与卡顿。

## 版本与成品

- 程序文件：KaoyaScreenshot.exe
- 产品版本：1.1.3；文件及程序集版本：1.1.3.0
- 文件大小：25,216,000 字节
- SHA-256：E216A04DA230525A42C8C983D17F9BF8F49DC291A5BEEAE45715A67B783AA291
- 公开下载：https://github.com/dianzihuang2/kaoya-screenshot-releases/releases/tag/v1.1.3
- 公开清单：https://github.com/dianzihuang2/kaoya-screenshot-releases/blob/main/update-v2.json
- 旧版 1.1.2 可自动识别 1.1.3 更新并提示升级；同版本不重复提示更新。

## 构建与验证

- 包含 RECORDING 和 FEATURE_TODO；未包含已停止的 PORTABLE_OCR。
- 录屏包 SHA-256：74799EEBEC38392FA0D3770897E4D9B444FEE75108C4BBCD8E387961739F745E
- 录屏对应源码：https://github.com/dianzihuang2/obs-kaoya/tree/ed9b3cc19f13d4adebd50a77d49114ae712f6c01
- Verify-DockExpand.ps1、Verify-MinimizeRestore.ps1、Verify-GlobalTodos.ps1、Verify-TodoReminders.ps1、Verify-TodoStage2.ps1、Verify-Release.ps1、TodoReminderSelfTest.exe 及录屏自测全数通过。
