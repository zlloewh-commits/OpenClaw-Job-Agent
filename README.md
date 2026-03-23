# OpenClaw Job Agent

This repository contains an anonymized version of my job application materials.

一个基于 OpenClaw 的 AI-native 求职投递 Agent，实现从简历生成到投递的自动化流程。

---

## 🚀 项目背景

在 AI-native 工作方式下，求职流程本身也可以被 Agent 重构。

本项目基于 OpenClaw 构建一个自动化投递 Agent，实现：

* 自动读取 Markdown 简历
* 基于岗位要求生成定制化投递内容
* 自动补全“为什么适合”等关键部分
* 支持通过通信渠道自动发送

---

## 🧠 核心能力

* **Agent 工作流设计**

  * resume → parsing → enhancement → application
* **Prompt + Workflow 结合**

  * 将岗位需求转化为结构化输出
* **模型能力利用**

  * 利用大模型进行信息补全与表达优化
* **工程化落地**

  * 使用 OpenClaw 实现可执行 Agent

---

## ⚙️ 技术栈

* OpenClaw（Agent框架）
* LLM（OpenAI / Claude / OpenRouter）
* Markdown（结构化输入输出）
* Workflow设计（AI-native）

---

## 🔄 工作流程

```text
resume.md
   ↓
Agent解析
   ↓
补全缺失信息
   ↓
生成 #JOB 投递格式
   ↓
发送给目标联系人
```

---

## 📄 示例输出

```md
#JOB
角色：大模型开发工程师
项目：...
为什么适合：...
```

---

## 📌 使用方式

```bash
openclaw agent \
  --agent job-agent \
  --message "读取resume.md生成#JOB投递内容"
```

---

## 💡 设计思考（加分点）

* 将“求职”抽象为一个可执行 workflow
* 将“表达能力”交给模型，“结构控制”由人完成
* 强调人机协同，而不是纯自动化

---

## 📬 作者

伍文豪
邮箱：[zlloewh@163.com](mailto:zlloewh@163.com)
