---
title: 小林 coding AI Agent 与 Claude Code 面试题
category: AI
description: 基于小林 coding 的 Agent、RAG、Claude Code 专题目录整理的 AI 工程化面试题索引。
tag:
  - AI
  - Agent
  - RAG
  - Claude Code
  - 面试题
---

本文件是题库索引型补充材料，来源于小林 coding 的 AI Agent 与 Claude Code 专题页。为了尊重原文版权，这里只保存题目、学习方向和原文链接，不离线复制完整长文与配图。刷到这些题时，建议先自己回答，再打开原文补齐细节。

## 图解 Agent · Agent 概念与生态

这组题主要考察 AI Agent 的基本定义、运行循环、工具调用、规划能力和开源生态理解。回答时不要只说“Agent 就是智能体”，要讲清楚它和普通 LLM 聊天的区别：Agent 会围绕目标进行感知、规划、执行和反馈，通常还会结合工具、记忆、环境状态与多轮任务控制。

参考来源：

- https://xiaolinnote.com/agent/concept/agent.html
- https://xiaolinnote.com/agent/concept/openclaw.html

高频面试题：

- AI Agent 是什么？它和普通大模型问答有什么区别？
- OpenClaw 是什么？它在 Agent 生态里解决了什么问题？

## 图解 Agent · RAG 检索增强

这组题主要考察 RAG 的基础链路、检索增强生成的价值、GraphRAG 和 LightRAG 的差异。回答时要把“检索、召回、重排、上下文注入、生成”串成完整流程，并能解释为什么 RAG 能缓解知识过时和幻觉问题，但不能彻底消除幻觉。

参考来源：

- https://xiaolinnote.com/agent/rag/rag.html
- https://xiaolinnote.com/agent/rag/graphrag-lightrag.html

高频面试题：

- RAG 是什么？一个完整的 RAG 问答流程通常包括哪些步骤？
- GraphRAG 和 LightRAG 有什么区别？实际项目中应该怎么选型？

## 图解 Agent · Agent 工程方法论

这组题主要考察 Agent 工程化方法论，包括 Harness Engineering 和 Loop Engineering。回答时可以从“让 Agent 可观测、可评估、可迭代、可反馈”展开，不要停留在写 prompt 的层面。

参考来源：

- https://xiaolinnote.com/agent/engineering/harness-engineering.html
- https://xiaolinnote.com/agent/engineering/loop-engineering.html

高频面试题：

- Harness Engineering 是什么？为什么说它能让 AI Agent 越用越聪明？
- Loop Engineering 是什么？它和传统 Prompt Engineering 有什么区别？

## 图解 Claude Code · 实战技巧

这组题主要考察 Claude Code 的日常使用能力，包括入门命令、项目记忆、官方互动课程和大型代码库协作。回答时可以结合自己的 Codex、Claude Code、Qwen Code 使用经历，重点说明如何读代码、拆任务、沉淀上下文和控制修改范围。

参考来源：

- https://xiaolinnote.com/claudecode/playbook/cc_use.html
- https://xiaolinnote.com/claudecode/playbook/cc_powerup.html
- https://xiaolinnote.com/claudecode/playbook/cc_claude_md.html
- https://xiaolinnote.com/claudecode/playbook/cc_large_codebase.html

高频面试题：

- Claude Code 新手入门时，最核心的使用流程是什么？
- Claude Code 的 /powerup 官方互动课程适合用来训练哪些能力？
- CLAUDE.md 应该怎么写？项目记忆文件通常要沉淀哪些内容？
- 面对百万行大型代码库，Claude Code 应该如何降低误改风险并提高定位效率？

## 图解 Claude Code · 源码解析

这组题主要考察 Claude Code 的架构理解，包括主循环、上下文压缩、代码检索、记忆机制和多 Agent。回答时可以从“模型不是单独工作，而是在工具、上下文、任务循环和安全边界里工作”这个角度展开。

参考来源：

- https://xiaolinnote.com/claudecode/source/cc_source.html
- https://xiaolinnote.com/claudecode/source/cc_query_loop.html
- https://xiaolinnote.com/claudecode/source/cc_compact.html
- https://xiaolinnote.com/claudecode/source/cc_grep.html
- https://xiaolinnote.com/claudecode/source/cc_memory.html
- https://xiaolinnote.com/claudecode/source/cc_multi_agent.html

高频面试题：

- Claude Code 的整体架构可以怎么拆解？一次代码任务通常会经过哪些模块？
- Claude Code 的主循环 Query 是怎么跑起来的？
- Claude Code 的 Compact 上下文压缩机制解决了什么问题？
- Claude Code 为什么偏向使用 grep 做代码检索，而不是默认使用 RAG？
- Claude Code 的记忆机制为什么不一定需要向量数据库？
- Claude Code 的 SubAgent 多 Agent 机制适合解决什么类型的问题？
