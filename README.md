# 优学院自动刷课脚本（JSON版本）

<div align="center">

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Mac%20%7C%20Linux-lightgrey.svg)

**湖南工学院专用 | 优学院自动学习辅助工具**

</div>

## 演示视频

📹 [点击观看使用教程](https://www.bilibili.com/video/BV1gddcBFECT)

<div align="center">
<iframe src="//player.bilibili.com/player.html?isOutside=true&aid=116533082720040&bvid=BV1gddcBFECT&cid=38162598839&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true" width="80%" height="450"></iframe>
</div>

> 💡 视频包含完整的安装和使用教程，建议首次使用时观看

## 功能特性

- **自动静音播放视频** - 自动静音播放每页视频
- **自动调整播放速率** - 支持自定义播放速度（0.25x - 15x）
- **自动翻页** - 视频播放完毕后自动跳转到下一节
- **自动作答** - 支持多种题型自动作答：
  - 单选题
  - 多选题
  - 判断题
  - 填空题/简答题
- **可视化配置面板** - 简洁易用的设置界面
- **答案显示** - 自动显示正确答案
- **配置持久化** - 设置自动保存，支持旧版本配置迁移

## 安装方法

### 前置条件

1. 安装浏览器扩展 **Tampermonkey**（推荐）或 **Greasemonkey**
   - [Chrome/Edge 安装 Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
   - [Firefox 安装 Tampermonkey](https://addons.mozilla.org/firefox/addon/tampermonkey/)

### 安装脚本

#### 方法一：从 Greasy Fork 安装（推荐）

访问 [Greasy Fork 脚本页面](https://update.greasyfork.org/scripts/396629) 直接安装

#### 方法二：手动安装

1. 点击浏览器工具栏的 Tampermonkey 图标
2. 选择「添加新脚本」
3. 删除编辑器中的默认内容
4. 将 `youxueyuan.js` 文件中的内容复制粘贴到编辑器中
5. 点击「文件」→「保存」

## 使用说明

1. 安装脚本后，访问优学院课程页面：
   - `https://ua.ulearning.cn/learnCourse/*`
   - `https://ua.dgut.edu.cn/learnCourse/*`

2. 脚本会自动运行，页面右上角会出现配置面板

3. 通过配置面板可以：
   - 开启/关闭自动播放
   - 调整播放速率
   - 开启/关闭自动答题
   - 设置各类题型的自动作答

## 配置选项

| 功能 | 说明 | 默认值 |
|------|------|--------|
| 自动翻页、播放视频 | 自动静音播放视频并翻页 | ✅ 开启 |
| 自动静音 | 视频自动静音播放 | ✅ 开启 |
| 自动调整速率 | 自动调整视频播放速度 | ✅ 开启 |
| 播放速率 | 视频播放速度 | 1.50x |
| 自动作答（总开关） | 自动作答所有题型 | ✅ 开启 |
| 自动显示答案 | 显示正确答案 | ✅ 开启 |
| 自动作答选择题 | 自动作答单选/多选题 | ✅ 开启 |
| 自动作答判断题 | 自动作答判断题 | ✅ 开启 |
| 自动作答填空/简答题 | 自动作答填空和简答题 | ✅ 开启 |

## 注意事项

> ⚠️ **免责声明**
>
> - 本脚本仅供学习交流使用
> - 请谨慎使用修改播放速率功能，产生的不良后果作者不承担任何责任
> - 请保持网课播放页面在浏览器中活动，避免长时间后台挂机
> - 脚本作者不提供任何保证，请自行判断使用风险

### 使用建议

1. **保持页面活动** - 避免最小化浏览器或切换到其他标签页过长时间
2. **刷新重试** - 如果脚本无效，请尝试刷新页面
3. **手动提交** - 关闭自动翻页功能后，答完题需要手动提交
4. **配置保存** - 修改设置后请点击「保存设置并刷新脚本」按钮

## 技术栈

- **JavaScript** - 核心脚本语言
- **jQuery** - DOM 操作
- **jQuery UI** - 拖拽功能
- **LocalStorage** - 配置持久化存储

## 项目结构

```
湖工优学院/
├── youxueyuan.js      # 主脚本文件
└── README.md          # 项目说明文档
```

> 📌 教学视频已上传至视频平台，可通过上方链接观看

## 更新日志

### v2.0.0 (2026-04-09)
- 重构代码架构，提升可维护性
- 新增配置管理器，支持配置持久化
- 新增日志管理器，便于调试
- 优化题目检测逻辑，提高答题准确率
- 支持从旧版本配置自动迁移
- 改进UI界面，提升用户体验

### v1.6.2
- 初始版本发布
- 基本功能实现

## 贡献者

- **EliotZhang** - 原作者
- **Brush-JIM** - 原作者
- **Claude Code** - 代码重构优化

## 许可证

本项目采用 [MIT 许可证](LICENSE) 开源

## 免责声明

本脚本是为方便学生学习而开发的辅助工具，仅供学习交流使用。使用本脚本产生的一切后果由使用者自行承担，脚本开发者不承担任何责任。请合理使用，遵守学校相关规定。

---

<div align="center">

**如果这个项目对你有帮助，请给个 ⭐ Star 支持一下！**

</div>