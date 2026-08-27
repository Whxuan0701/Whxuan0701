# Wei Haoxuan

> Harbin University of Science and Technology<br>
> Agent开发 / 后端开发<br>
> GitHub: [@Whxuan0701](https://github.com/Whxuan0701)

关注 AI Agent 工程、后端系统与可靠性，希望把 Agent 从“可以运行”推进到“可验证、可恢复、可观测”。

在研 APGFR: Prior-Guided Sparse-View Gaussian Reconstruction （3D Gaussian）

## About Me

- 学校：哈尔滨理工大学
- 专业：大数据
- 研究方向：Agent工程 / 大模型 / 计算机视觉 / 多模态Agent
- 当前关注：AI Agent、skill、Agent Runtime、RAG
- 技术栈：Python / TypeScript / Go / Java
- 邮箱：641627652@qq.com


## Open-source Snapshot

截至 2026-08-26，GitHub 公开记录中：

- 向 **32 个仓库**提出 **91 个 Pull Requests**，其中 **90 个是外部仓库贡献**
- **28 个已合并**，**55 个仍开放**，**8 个已关闭**；开放项中包含仍处于 Draft 的工作
- 向 **6 个 Apache 仓库**提出 **9 个 PR**：3 个已合并、5 个仍开放、1 个已关闭


## Representative Contributions

### 1. Agent Runtime: bounded execution and recovery

在 [buildwithclaude](https://github.com/davepoon/buildwithclaude) [![GitHub Stars](https://img.shields.io/github/stars/davepoon/buildwithclaude?style=flat&label=stars)](https://github.com/davepoon/buildwithclaude) 中实现并合并：

- [`checkpointed-agent-loop`](https://github.com/davepoon/buildwithclaude/pull/278)：为长任务提供版本化检查点、有限状态机、重试预算、原子写入、恢复入口和验证证据；脚本只负责状态，不执行命令或访问网络。
- [`rag-evaluation-harness`](https://github.com/davepoon/buildwithclaude/pull/279)：实现确定性、离线的 RAG 评测工具，计算 Recall@K、MRR、Context Precision、Citation Coverage/Validity，并用退出码支持 CI 阈值门禁。

在 Apache Agent 框架 [Burr](https://github.com/apache/burr) [![GitHub Stars](https://img.shields.io/github/stars/apache/burr?style=flat&label=stars)](https://github.com/apache/burr) 中提交的进行中贡献：

- [`InMemoryExecutionRecorder`](https://github.com/apache/burr/pull/890)：通过生命周期钩子记录 Agent 的 action、输入、结果、异常和状态变化，用于本地回放与测试。
- [`Graph.to_dict()`](https://github.com/apache/burr/pull/891)：提供无需 Graphviz 或 tracking 依赖的确定性图结构导出。
- [`max_steps` execution budget](https://github.com/apache/burr/pull/892)：为同步/异步执行与迭代接口增加单次执行步数预算，在 Agent Loop 未自然结束时安全失败并保留可恢复状态。

### 2. Multi-agent isolation and orchestration safety

在 [kagent](https://github.com/kagent-dev/kagent) [![GitHub Stars](https://img.shields.io/github/stars/kagent-dev/kagent?style=flat&label=stars)](https://github.com/kagent-dev/kagent) 中实现并合并：

- [`isolateSessions` for remote agent tools](https://github.com/kagent-dev/kagent/pull/2504)：让并发远程 A2A 调用按配置创建独立上下文，避免多个子 Agent 共享可变 Session 状态。
- [Agent Plugin skill selection hardening](https://github.com/kagent-dev/kagent/pull/2505)：在下载制品前拒绝路径穿越式名称、路径分隔符和重复 Skill，避免覆盖与非确定性物化。

在 [llama-agents](https://github.com/run-llama/llama-agents) [![GitHub Stars](https://img.shields.io/github/stars/run-llama/llama-agents?style=flat&label=stars)](https://github.com/run-llama/llama-agents) 中实现并合并：

- [拒绝并发复用活跃 Handler ID](https://github.com/run-llama/llama-agents/pull/738)：为阻塞与非阻塞接口返回稳定的 `409 Conflict`，同时保留终态 ID 的复用能力。
- [WorkflowClient 类型化工作流内省](https://github.com/run-llama/llama-agents/pull/739)：暴露输入/输出 Schema、事件 Schema 与工作流图结构，并补充客户端集成测试。

### 3. MCP client and inspection tooling

在 [mcp-use](https://github.com/mcp-use/mcp-use) [![GitHub Stars](https://img.shields.io/github/stars/mcp-use/mcp-use?style=flat&label=stars)](https://github.com/mcp-use/mcp-use) 中实现并合并：

- [`RequestOptions` for prompt reads](https://github.com/mcp-use/mcp-use/pull/2302)：为 Prompt 请求补齐超时、取消和进度回调能力，并保持原有双参数接口兼容。
- [Inspector RPC response correlation](https://github.com/mcp-use/mcp-use/pull/2303)：按 JSON-RPC ID、来源、方向和组件关联请求与响应，在 Inspector 中展示方法名、耗时和错误状态。

其他 MCP/SDK 方向的贡献还覆盖工具命名空间、任务轮询、Roots Handler、MCP 初始化就绪检查、机器可读输出与跨 Agent Trace 传播，完整状态见 [PR Ledger](./OPEN_SOURCE_PR_LEDGER.md)。

### 4. Agent evaluation, evidence and failure testing

在 [agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) [![GitHub Stars](https://img.shields.io/github/stars/sickn33/agentic-awesome-skills?style=flat&label=stars)](https://github.com/sickn33/agentic-awesome-skills) 中合并 5 项 Agent 工程方法：

- [Agent 评测报告](https://github.com/sickn33/agentic-awesome-skills/pull/1177)
- [跨平台契约传播审计](https://github.com/sickn33/agentic-awesome-skills/pull/1178)
- [Agent Harness 故障注入](https://github.com/sickn33/agentic-awesome-skills/pull/1189)
- [Agent Run 证据审计](https://github.com/sickn33/agentic-awesome-skills/pull/1192)
- [多智能体编排评审](https://github.com/sickn33/agentic-awesome-skills/pull/1193)

这些工作把多 Agent 编排视为分布式状态机，重点检查所有权、租约与 fencing、版本化状态、分支 Join、重试与幂等、取消、预算、检查点恢复以及“验证制品与部署制品是否一致”。

### 5. RAG and code intelligence reliability

在 [code-graph-rag](https://github.com/vitali87/code-graph-rag) [![GitHub Stars](https://img.shields.io/github/stars/vitali87/code-graph-rag?style=flat&label=stars)](https://github.com/vitali87/code-graph-rag) 中合并 3 个可靠性修复：

- [目录结果确定性排序](https://github.com/vitali87/code-graph-rag/pull/1309)
- [拒绝无效源码位置范围](https://github.com/vitali87/code-graph-rag/pull/1310)
- [拒绝越界、反向及路径穿越式代码片段请求](https://github.com/vitali87/code-graph-rag/pull/1311)

这些改动避免文件系统顺序、陈旧图位置和非法范围影响 Agent 的检索结果，使下游 RAG/代码理解流程获得更稳定、可信的上下文。

### 6. Search, CLI and workflow engineering

- [buildwithclaude #270](https://github.com/davepoon/buildwithclaude/pull/270) [![GitHub Stars](https://img.shields.io/github/stars/davepoon/buildwithclaude?style=flat&label=stars)](https://github.com/davepoon/buildwithclaude)、[#271](https://github.com/davepoon/buildwithclaude/pull/271)、[#272](https://github.com/davepoon/buildwithclaude/pull/272)：处理 YAML 日期归一化、搜索对象 ID 冲突，以及 Plugin/Skill 同名时的检索结果身份保持。
- [OpenCLI #2298](https://github.com/jackwener/OpenCLI/pull/2298) [![GitHub Stars](https://img.shields.io/github/stars/jackwener/OpenCLI?style=flat&label=stars)](https://github.com/jackwener/OpenCLI)、[#2299](https://github.com/jackwener/OpenCLI/pull/2299)、[#2300](https://github.com/jackwener/OpenCLI/pull/2300)：增强无效 Manifest 回退、`<1.0.0` caret 版本范围及整数参数校验。
- [planning-with-files #222](https://github.com/OthmanAdi/planning-with-files/pull/222) [![GitHub Stars](https://img.shields.io/github/stars/OthmanAdi/planning-with-files?style=flat&label=stars)](https://github.com/OthmanAdi/planning-with-files)、[#223](https://github.com/OthmanAdi/planning-with-files/pull/223)、[#224](https://github.com/OthmanAdi/planning-with-files/pull/224)：修复 Copilot PowerShell Hook、禁用开关传播与 Python 解释器一致性。

### 7. Apache contributions

已合并：

- [Apache Magpie #1112](https://github.com/apache/magpie/pull/1112) [![GitHub Stars](https://img.shields.io/github/stars/apache/magpie?style=flat&label=stars)](https://github.com/apache/magpie)：明确本地配置覆盖优先级与 additive-only 安全边界。
- [Apache Magpie #1113](https://github.com/apache/magpie/pull/1113) [![GitHub Stars](https://img.shields.io/github/stars/apache/magpie?style=flat&label=stars)](https://github.com/apache/magpie)：修正文档对 Reviewer Routing 覆盖能力的表述。
- [Apache Cordova Docs #1519](https://github.com/apache/cordova-docs/pull/1519) [![GitHub Stars](https://img.shields.io/github/stars/apache/cordova-docs?style=flat&label=stars)](https://github.com/apache/cordova-docs)：澄清 Android Vector/Adaptive Icon 的转换与使用说明。

审阅中：

- [Apache Burr #890-#892](https://github.com/pulls?q=is%3Apr+author%3AWhxuan0701+repo%3Aapache%2Fburr) [![GitHub Stars](https://img.shields.io/github/stars/apache/burr?style=flat&label=stars)](https://github.com/apache/burr)：执行记录、图序列化与执行步数预算。
- [Apache Camel K #6773](https://github.com/apache/camel-k/pull/6773) [![GitHub Stars](https://img.shields.io/github/stars/apache/camel-k?style=flat&label=stars)](https://github.com/apache/camel-k)：补充多命名空间安装方式文档。
- [Apache Fineract Backoffice UI #449](https://github.com/apache/fineract-backoffice-ui/pull/449) [![GitHub Stars](https://img.shields.io/github/stars/apache/fineract-backoffice-ui?style=flat&label=stars)](https://github.com/apache/fineract-backoffice-ui)：适配生成后的 Floating Rate Request 类型。

## Engineering Principles

- **Bounded execution**：循环、重试和并发必须有明确预算及终止条件。
- **Recoverable state**：检查点要可验证、可恢复，并区分业务状态与尝试记录。
- **Evidence before claims**：完成状态必须绑定测试、Trace、Artifact 或可复现输出。
- **Protocol compatibility**：扩展 MCP/SDK 接口时保留兼容路径，明确取消、超时与错误语义。
- **Deterministic behavior**：排序、标识符、序列化和状态转换应可重复验证。
- **Honest boundaries**：Open、Draft、Closed 与 Merged 分开呈现；局部测试不等同于全仓库或生产验证。

## Current Focus

- 3D Gaussian
- ReAct
- Dynamic Patch Perception

## Contact

- Email: 641627652@qq.com


完整的 91 个 PR、仓库分布及当前状态：[`OPEN_SOURCE_PR_LEDGER.md`](./OPEN_SOURCE_PR_LEDGER.md)
