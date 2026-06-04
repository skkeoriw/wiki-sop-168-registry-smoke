---
```yaml
title: Sonnet
type: entity
tags:
  - Claude
  - 模型
  - Dynamic Workflows
  - 代码审查
summary: Sonnet 是 Claude 模型系列中的一个模型，常用于 Dynamic Workflows 中的对抗验证阶段，以兼顾逻辑能力与速度。
sources:
  - raw/notebooklm-analysis/Claude-Code-Dynamic-Workflows-高级用法与实践简报.md
created: 2024-04-17
updated: 2024-04-17
layer: L1
confidence: high
reasoning: Sonnet 在报告中被明确提及为一个模型，并在成本与性能优化策略的表格中被列为建议模型，用于对抗验证阶段。其在场景三中也与 Codex CLI 和 Opus 模型一同被提及，作为独立审查任务的一部分。
---
Sonnet 是 Claude 模型系列中的一个重要组成部分，在 [[Claude Code Dynamic Workflows 高级用法与实践简报]] 中扮演着关键角色。它通常被部署在 Dynamic Workflows 的第三阶段，即“对抗验证”阶段。在这个阶段，Sonnet 的主要作用是兼顾分析的逻辑能力与执行速度，为代码审查提供一个高效且具备一定深度的验证能力。与 [[Opus]] 模型（通常用于报告合成，追求最终产出的准确性与权威性）和 [[Haiku]] 模型（用于初步分析，以极低的成本处理海量数据）相比，Sonnet 提供了性能上的平衡。

在 [[Codex CLI]] 交叉验证代码审查的场景中，Sonnet 与 Codex CLI 和 Opus 模型一同被启动，形成“三方协同”的审查机制。这种多模型协作的策略旨在利用不同模型的互补优势，例如 Codex CLI 对特定代码逻辑的敏感度，以发现 Claude 模型系列（包括 Sonnet 和 Opus）可能忽略的潜在 Bug。通过这种方式，可以实现更全面、更深入的代码审查，提升代码质量。实测数据显示，与 Opus/Sonnet 模型动辄 100K+ 的 Token 消耗相比，调用 Codex CLI 的智能体仅消耗 20K Token，这表明 Sonnet 在提供分析能力的同时，也需要考虑 Token 消耗的成本效益。因此，在 Dynamic Workflows 的设计中，将 Sonnet 安排在对抗验证阶段，是基于其在成本与性能之间取得良好平衡的考量。
```