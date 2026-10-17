# 取经计划 · 项目管理四级训练营（私有全量镜像）

《西游记·ICT 项目管理》培训课程的**私有全量备份镜像**（含音频等未发布素材），与公开发布仓实时同步。

## 三仓体系

| 仓库 | 平台 | 可见性 | 用途 |
|---|---|---|---|
| [mousejl/xiyou-ict-pm](https://github.com/mousejl/xiyou-ict-pm) | GitHub | **公开** | 线上发布站（GitHub Pages：https://mousejl.github.io/xiyou-ict-pm/ ） |
| **本仓库** training-materials | Gitee | **私有** | 课程全量镜像（第一备份端） |
| mousejl/training-materials-private | GitHub | **私有** | 课程全量镜像（第二备份端） |

本地工作目录 `git push origin main` 一次推送自动同步三端。

> 服务器端考试系统（题库/教师版试卷/成绩数据库）**不在本仓库**，独立备份于 `exam-report-backup` 私有双仓——题库含答案、试卷含答案，绝不入本仓库与公开仓。

## 内容清单

| 目录/文件 | 说明 |
|---|---|
| `curriculum/` | **新版课程主体**（取经计划） |
| ├ `index.html` | 统一入口页（课件导航 + 主讲老师专区：老师登记/开考控制台 + 通关文牒体系） |
| ├ `g0.html`~`c4.html` | 五门课件（通识全景 L+ / 认知 L1 / 基础 L2 / 实战 L3 / 治理 L4，共 66 页） |
| ├ `speech-*.html` | 各门口播稿（含通识课标准版/脱口秀版共 6 份） |
| ├ `audio/` | 各门口播音频（g0/g0-fun/c1~c4，分段+合并版 mp3） |
| ├ `exams/` | 五门结业试卷（公开版**不含答案**）+ 在线答题页 quiz.html + 开考二维码 SVG |
| ├ `score.html` | 成绩查询（学员凭手机号查本人成绩 / 老师凭登记手机号查全班） |
| ├ `test.html` | 角色自测 H5（测你是师徒五人中的谁） |
| ├ `passport.html` | 通关文牒（古风结业凭证，≥95 分自动发放 PDF） |
| ├ `templates.html` | 八份随堂教具模板（登记册/纪要/三栏清单等，支持打印） |
| └ `seal/` `fonts/` | 五级印章 SVG 与站酷小薇字体 |
| `course/` | **经典版** 25 页全景课件（旧版存档，与新版并存） |
| `speech*.html`（根部） | 经典版各版口播稿（全集/趣味/脱口秀/演讲版） |
| `audio/`（根部） | 经典版口播音频（40 段 mp3，约 29M） |

## 关键机制

- **结业考试仅课堂扫码**：开考由老师在统一入口"主讲老师专区"→开考控制台操作（每场单一科目二维码 + 实时交卷数 + 分享链接）；学生无任何自助考试入口
- **教师版试卷/答案/题库**：仅存 `exam-report-backup` 私有仓，公开站点与公开仓零答案
- **老师登录体系**：主讲老师手机号登记（登记口令 admin 圈内传达）→ 同一手机号通用于开考控制台、成绩查询（老师端）、成绩总表

## 恢复方法

任一端故障时，从另一私有端克隆即可完整找回（含全部历史）：

```bash
git clone https://gitee.com/mousejl/training-materials.git
# 或：git clone https://github.com/mousejl/training-materials-private.git
```

恢复线上站：克隆后将 `main` 推回 GitHub `xiyou-ict-pm`，GitHub Pages 自动重新部署（约 1-2 分钟）。

## 同步状态

- 本镜像与公开仓内容逐字节一致（同一次推送的三个远端）
- 最近更新见提交记录；线上站点验活地址：https://mousejl.github.io/xiyou-ict-pm/

> AI生成
