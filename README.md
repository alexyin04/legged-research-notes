# 四足机器人学习笔记

> A learning notebook on quadruped locomotion, DreamWaQ, sim2real, and evaluation, grounded in a 12-DOF robot project.

这里记录我在四足机器人项目中学到的知识、十次改进过程，以及实验里遇到的问题。内容会随理解和实验持续修订。

## 内容分区

| 分区 | 内容 | 当前状态 |
| --- | --- | --- |
| **knowledge/** | DreamWaQ 原理、sim2real 基础 | 已写 2 篇，后续按学习进度补充 |
| **journey/** | 十次迭代的改动、原因和结果 | 已有完整时间线，后续补证据链接 |
| **engineering/** | 踩坑清单、泛化性评测方法 | 已写 2 篇，随新实验更新 |
| **papers/** | 读过的论文和判断 | 索引草稿，部分信息标为 `[待核]` |
| **problems/** | 开放问题、实验数据和自己的判断 | 问题 1–3 已有正文，4–7 待写 |

## 从哪开始

- 了解方法：[DreamWaQ 学习笔记](knowledge/dreamwaq.md)
- 了解仿真到真机：[sim2real 学习笔记](knowledge/sim2real.md)
- 看项目怎么一步步改出来：[十次迭代](journey/iterations.md)
- 看具体工程问题：[25 个坑](engineering/pitfalls.md)
- 看实验怎么设计：[泛化性评测](engineering/evaluation.md)

## 内容约定

- 实验数字来自这台 12 自由度四足机器人及对应策略，不能直接推广到其他硬件。
- 个人判断用“我认为”标出，并与测量结果分开。
- 论文信息没有回到原文确认的，保留 `[待核]`；没有内容的页面明确标为“待写”。
- 公开版本只放已有工作、通用知识和可公开实验记录。

后续填充顺序和站点优化条件见 [维护路线](ROADMAP.md)。

## 本地预览

安装 Python 3 后，在本目录运行：

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

然后访问 `http://127.0.0.1:8000`。网站由 Docsify 在浏览器中渲染，无需构建。Docsify 4.13.1 的脚本和样式已随仓库提供，预览不依赖 CDN。

## 相关项目

代码、配置和测试在主仓库：[dreamwaq-quadruped](https://github.com/alexyin04/dreamwaq-quadruped)。
