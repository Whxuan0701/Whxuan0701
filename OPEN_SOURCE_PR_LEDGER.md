# Open-source Pull Request Ledger

GitHub account: [Whxuan0701](https://github.com/Whxuan0701)<br>
Snapshot date: 2026-08-26<br>
Query: [`is:pr author:Whxuan0701`](https://github.com/pulls?q=is%3Apr+author%3AWhxuan0701)

## Scope and Status Rules

- 本清单收录 GitHub 公开检索到的全部 **91 个 PR**，分布于 **32 个仓库**。
- 其中 **28 MERGED / 55 OPEN / 8 CLOSED**；12 个 PR 当前为 Draft。
- 共有 **90 个外部仓库 PR**，另有 1 个账号自有仓库 Draft PR。
- TapTap 项目没有出现在 `author:Whxuan0701` 的公开 PR 结果中，本清单也未纳入任何 TapTap 工作。
- `OPEN` 仅表示仍在审阅或等待处理，不表示已被维护者认可；`CLOSED` 也不等同于合并。

## Complete Ledger

### Agent frameworks and runtimes

#### apache/burr - 3 PRs

- `OPEN` [#890 feat(lifecycle): add in-memory execution recorder](https://github.com/apache/burr/pull/890)
- `OPEN` [#891 feat(core): add dependency-free graph serialization](https://github.com/apache/burr/pull/891)
- `OPEN` [#892 feat(core): add execution step budgets](https://github.com/apache/burr/pull/892)

#### kagent-dev/kagent - 3 PRs

- `MERGED` [#2504 feat(python-adk): honor isolateSessions for remote agent tools](https://github.com/kagent-dev/kagent/pull/2504)
- `MERGED` [#2505 fix(agentplugins): reject unsafe and conflicting skill selections](https://github.com/kagent-dev/kagent/pull/2505)
- `OPEN` [#2506 feat(adk): retain MCP server identities in runtime diagnostics](https://github.com/kagent-dev/kagent/pull/2506)

#### run-llama/llama-agents - 3 PRs

- `OPEN` [#737 Add handler completion polling to WorkflowClient](https://github.com/run-llama/llama-agents/pull/737)
- `MERGED` [#738 Reject concurrent reuse of active handler IDs](https://github.com/run-llama/llama-agents/pull/738)
- `MERGED` [#739 Add typed workflow introspection to WorkflowClient](https://github.com/run-llama/llama-agents/pull/739)

#### ag2ai/ag2 - 3 PRs

- `OPEN` [#3180 feat(subagents): bound concurrent task fan-out](https://github.com/ag2ai/ag2/pull/3180)
- `OPEN` [#3181 fix(skills): execute nested scripts from declared paths](https://github.com/ag2ai/ag2/pull/3181)
- `OPEN` [#3182 feat(mcp): support namespaced toolkit tools](https://github.com/ag2ai/ag2/pull/3182)

#### SWE-agent/SWE-agent - 3 PRs

- `OPEN` [#1512 Add side-effect-free replay preflight validation](https://github.com/SWE-agent/SWE-agent/pull/1512)
- `OPEN` [#1513 Add machine-readable JSON output to quick-stats](https://github.com/SWE-agent/SWE-agent/pull/1513)
- `OPEN` [#1514 Expose retry attempt lifecycle hooks](https://github.com/SWE-agent/SWE-agent/pull/1514)

#### langroid/langroid - 3 PRs

- `CLOSED / DRAFT` [#1090 feat(mcp): namespace tools from multiple servers](https://github.com/langroid/langroid/pull/1090)
- `CLOSED / DRAFT` [#1091 feat(task): add cooperative wall-clock budgets](https://github.com/langroid/langroid/pull/1091)
- `CLOSED / DRAFT` [#1092 feat(agent): add portable chat history snapshots](https://github.com/langroid/langroid/pull/1092)

#### getzep/graphiti - 3 PRs

- `OPEN` [#1783 feat(llm): add optional timeout and extra_body to LLMConfig](https://github.com/getzep/graphiti/pull/1783)
- `OPEN` [#1784 fix(dedupe): make edge contradiction reasoning explicit](https://github.com/getzep/graphiti/pull/1784)
- `OPEN` [#1785 fix(nodes): persist and restore episodic metadata](https://github.com/getzep/graphiti/pull/1785)

#### mastra-ai/mastra - 1 PR

- `CLOSED` [#22268 test(core): cover idempotent channel initialization](https://github.com/mastra-ai/mastra/pull/22268)

#### calesthio/OpenMontage - 5 PRs

- `OPEN` [#338 refactor: Unify .env loading logic, eliminate code duplication](https://github.com/calesthio/OpenMontage/pull/338)
- `OPEN` [#342 feat: Add unified logging system](https://github.com/calesthio/OpenMontage/pull/342)
- `OPEN` [#343 feat: Add tool contract validation mechanism](https://github.com/calesthio/OpenMontage/pull/343)
- `OPEN` [#344 feat: Add tool health check and warmup functionality](https://github.com/calesthio/OpenMontage/pull/344)
- `OPEN` [#345 feat: Add performance metrics collection system](https://github.com/calesthio/OpenMontage/pull/345)

#### zhayujie/CowAgent - 3 PRs

- `OPEN / DRAFT` [#3061 fix(keyword): detect attachment URLs by parsed path](https://github.com/zhayujie/CowAgent/pull/3061)
- `OPEN / DRAFT` [#3062 fix(scheduler): prevent concurrent task updates from being lost](https://github.com/zhayujie/CowAgent/pull/3062)
- `OPEN / DRAFT` [#3063 fix(skill): harden tar archive extraction](https://github.com/zhayujie/CowAgent/pull/3063)

### MCP, SDK and observability

#### mcp-use/mcp-use - 2 PRs

- `MERGED` [#2302 feat(client): support RequestOptions for prompt reads](https://github.com/mcp-use/mcp-use/pull/2302)
- `MERGED` [#2303 feat(inspector): correlate RPC response labels](https://github.com/mcp-use/mcp-use/pull/2303)

#### mark3labs/mcp-go - 3 PRs

- `OPEN` [#953 feat(client): configure in-process host handlers together](https://github.com/mark3labs/mcp-go/pull/953)
- `OPEN` [#954 feat(client): add context-aware task polling helper](https://github.com/mark3labs/mcp-go/pull/954)
- `OPEN` [#955 feat(mcptest): add roots handler support](https://github.com/mark3labs/mcp-go/pull/955)

#### stacklok/toolhive - 3 PRs

- `OPEN` [#6373 Annotate vMCP optimizer discovery tool](https://github.com/stacklok/toolhive/pull/6373)
- `OPEN` [#6374 Add an MCP initialize readiness check](https://github.com/stacklok/toolhive/pull/6374)
- `OPEN` [#6381 Add JSON output to vMCP validation](https://github.com/stacklok/toolhive/pull/6381)

#### traceloop/openllmetry - 3 PRs

- `OPEN` [#4433 fix(sdk): keep oversized entity attributes exportable](https://github.com/traceloop/openllmetry/pull/4433)
- `OPEN` [#4434 feat(sdk): add W3C agent trace propagation helpers](https://github.com/traceloop/openllmetry/pull/4434)
- `OPEN` [#4435 feat(gnap): add agent coordination instrumentation](https://github.com/traceloop/openllmetry/pull/4435)

#### superradcompany/microsandbox - 3 PRs

- `OPEN / DRAFT` [#1395 feat(cli): add JSON output to exec](https://github.com/superradcompany/microsandbox/pull/1395)
- `OPEN` [#1396 feat(cli): add sandbox wait command](https://github.com/superradcompany/microsandbox/pull/1396)
- `OPEN / DRAFT` [#1397 feat(cli): add JSON output to ping](https://github.com/superradcompany/microsandbox/pull/1397)

#### discourse/discourse - 3 PRs

- `OPEN / DRAFT` [#42671 FEATURE: Support paginated MCP tool discovery](https://github.com/discourse/discourse/pull/42671)
- `OPEN / DRAFT` [#42672 UX: Sync MCP health after connection tests](https://github.com/discourse/discourse/pull/42672)
- `OPEN / DRAFT` [#42674 DEV: Add an eval run limit](https://github.com/discourse/discourse/pull/42674)

### Agent skills, evaluation and developer tooling

#### davepoon/buildwithclaude - 6 PRs

- `MERGED` [#270 Update story parsing: normalize YAML dates](https://github.com/davepoon/buildwithclaude/pull/270)
- `MERGED` [#271 Update search object IDs: prevent sanitized slug collisions](https://github.com/davepoon/buildwithclaude/pull/271)
- `MERGED` [#272 Update search hydration: preserve plugin and skill identity](https://github.com/davepoon/buildwithclaude/pull/272)
- `CLOSED` [#277 Add MCP project config export](https://github.com/davepoon/buildwithclaude/pull/277)
- `MERGED` [#278 Add checkpointed-agent-loop skill](https://github.com/davepoon/buildwithclaude/pull/278)
- `MERGED` [#279 Add rag-evaluation-harness skill](https://github.com/davepoon/buildwithclaude/pull/279)

#### sickn33/agentic-awesome-skills - 7 PRs

- `MERGED` [#1177 feat: add agent evaluation reporting skill](https://github.com/sickn33/agentic-awesome-skills/pull/1177)
- `MERGED` [#1178 feat: add cross-platform contract propagation audit skill](https://github.com/sickn33/agentic-awesome-skills/pull/1178)
- `CLOSED` [#1187 feat: add stack artifact audit](https://github.com/sickn33/agentic-awesome-skills/pull/1187)
- `CLOSED` [#1188 feat: add paired Workbench artifact review](https://github.com/sickn33/agentic-awesome-skills/pull/1188)
- `MERGED` [#1189 feat: add agent harness fault injection skill](https://github.com/sickn33/agentic-awesome-skills/pull/1189)
- `MERGED` [#1192 feat: add agent run evidence audit skill](https://github.com/sickn33/agentic-awesome-skills/pull/1192)
- `MERGED` [#1193 feat: add multi-agent orchestration review skill](https://github.com/sickn33/agentic-awesome-skills/pull/1193)

#### Jeffallan/claude-skills - 3 PRs

- `OPEN` [#231 feat(skills): add accessibility engineer](https://github.com/Jeffallan/claude-skills/pull/231)
- `OPEN` [#232 feat(validation): enforce documentation backlinks](https://github.com/Jeffallan/claude-skills/pull/232)
- `OPEN` [#233 feat(tooling): add skill scaffold generator](https://github.com/Jeffallan/claude-skills/pull/233)

#### yusufkaraaslan/Skill_Seekers - 3 PRs

- `OPEN` [#457 feat(cli): add read-only source detection command](https://github.com/yusufkaraaslan/Skill_Seekers/pull/457)
- `OPEN` [#458 feat(quality): support JSON reports on stdout](https://github.com/yusufkaraaslan/Skill_Seekers/pull/458)
- `OPEN` [#459 feat(doctor): add machine-readable JSON output](https://github.com/yusufkaraaslan/Skill_Seekers/pull/459)

#### NirDiamant/GenAI_Agents - 3 PRs

- `OPEN` [#134 Add human-in-the-loop approval agent tutorial](https://github.com/NirDiamant/GenAI_Agents/pull/134)
- `OPEN` [#135 Add trace-based agent evaluation tutorial](https://github.com/NirDiamant/GenAI_Agents/pull/135)
- `OPEN` [#136 Add notebook contribution validator](https://github.com/NirDiamant/GenAI_Agents/pull/136)

#### NirDiamant/agents-towards-production - 3 PRs

- `OPEN` [#79 fix: declare PyPDF2 for the Streamlit tutorial](https://github.com/NirDiamant/agents-towards-production/pull/79)
- `OPEN` [#80 fix: declare pandas for the agent security tutorial](https://github.com/NirDiamant/agents-towards-production/pull/80)
- `OPEN` [#81 test: fix FastAPI streaming response assertions](https://github.com/NirDiamant/agents-towards-production/pull/81)

### RAG, repository intelligence and CLI reliability

#### vitali87/code-graph-rag - 3 PRs

- `MERGED` [#1309 fix: return deterministic directory listings](https://github.com/vitali87/code-graph-rag/pull/1309)
- `MERGED` [#1310 fix: reject invalid source location ranges](https://github.com/vitali87/code-graph-rag/pull/1310)
- `MERGED` [#1311 fix: reject invalid code snippet spans](https://github.com/vitali87/code-graph-rag/pull/1311)

#### yamadashy/repomix - 3 PRs

- `OPEN` [#1808 fix(cli): Reject split sizes below one byte](https://github.com/yamadashy/repomix/pull/1808)
- `OPEN` [#1809 fix(cli): Respect directory boundaries when classifying paths](https://github.com/yamadashy/repomix/pull/1809)
- `OPEN` [#1810 fix(skill): Derive repository names from GitHub URLs](https://github.com/yamadashy/repomix/pull/1810)

#### jackwener/OpenCLI - 3 PRs

- `MERGED` [#2298 fix(completion): fall back on invalid manifests](https://github.com/jackwener/OpenCLI/pull/2298)
- `MERGED` [#2299 fix(plugin): honor caret ranges below 1.0.0](https://github.com/jackwener/OpenCLI/pull/2299)
- `MERGED` [#2300 fix(args): reject invalid integer values](https://github.com/jackwener/OpenCLI/pull/2300)

#### OthmanAdi/planning-with-files - 3 PRs

- `MERGED` [#222 fix: ignore unstructured plans in Copilot PowerShell stop hook](https://github.com/OthmanAdi/planning-with-files/pull/222)
- `MERGED` [#223 fix: honor PLANNING_DISABLED in GitHub Copilot hooks](https://github.com/OthmanAdi/planning-with-files/pull/223)
- `MERGED` [#224 test: run Hermes probe with the active Python interpreter](https://github.com/OthmanAdi/planning-with-files/pull/224)

### Apache documentation and application projects

#### apache/magpie - 2 PRs

- `MERGED` [#1112 docs: document local override precedence](https://github.com/apache/magpie/pull/1112)
- `MERGED` [#1113 docs(spec-loop): align reviewer-routing coverage claim](https://github.com/apache/magpie/pull/1113)

#### apache/cordova-docs - 1 PR

- `MERGED` [#1519 docs: clarify Android vector icon guidance](https://github.com/apache/cordova-docs/pull/1519)

#### apache/camel-k - 1 PR

- `OPEN` [#6773 docs: Document multi-namespace installation methods](https://github.com/apache/camel-k/pull/6773)

#### apache/fineract-backoffice-ui - 1 PR

- `OPEN` [#449 fix(api): adapt floating rate form to generated request types](https://github.com/apache/fineract-backoffice-ui/pull/449)

#### apache/security-dash - 1 PR

- `CLOSED` [#9 docs: link security dashboard source and issues](https://github.com/apache/security-dash/pull/9)

### Personal repository

#### Whxuan0701/true-cost-chrome-extension - 1 PR

- `OPEN / DRAFT` [#1 Harden True Cost release baseline](https://github.com/Whxuan0701/true-cost-chrome-extension/pull/1)

## Summary by Repository

| Repository | Total | Merged | Open | Closed |
|---|---:|---:|---:|---:|
| davepoon/buildwithclaude | 6 | 5 | 0 | 1 |
| sickn33/agentic-awesome-skills | 7 | 5 | 0 | 2 |
| calesthio/OpenMontage | 5 | 0 | 5 | 0 |
| apache/burr | 3 | 0 | 3 | 0 |
| kagent-dev/kagent | 3 | 2 | 1 | 0 |
| run-llama/llama-agents | 3 | 2 | 1 | 0 |
| vitali87/code-graph-rag | 3 | 3 | 0 | 0 |
| jackwener/OpenCLI | 3 | 3 | 0 | 0 |
| OthmanAdi/planning-with-files | 3 | 3 | 0 | 0 |
| ag2ai/ag2 | 3 | 0 | 3 | 0 |
| SWE-agent/SWE-agent | 3 | 0 | 3 | 0 |
| langroid/langroid | 3 | 0 | 0 | 3 |
| getzep/graphiti | 3 | 0 | 3 | 0 |
| zhayujie/CowAgent | 3 | 0 | 3 | 0 |
| mark3labs/mcp-go | 3 | 0 | 3 | 0 |
| stacklok/toolhive | 3 | 0 | 3 | 0 |
| traceloop/openllmetry | 3 | 0 | 3 | 0 |
| superradcompany/microsandbox | 3 | 0 | 3 | 0 |
| discourse/discourse | 3 | 0 | 3 | 0 |
| Jeffallan/claude-skills | 3 | 0 | 3 | 0 |
| yusufkaraaslan/Skill_Seekers | 3 | 0 | 3 | 0 |
| NirDiamant/GenAI_Agents | 3 | 0 | 3 | 0 |
| NirDiamant/agents-towards-production | 3 | 0 | 3 | 0 |
| yamadashy/repomix | 3 | 0 | 3 | 0 |
| mcp-use/mcp-use | 2 | 2 | 0 | 0 |
| apache/magpie | 2 | 2 | 0 | 0 |
| apache/cordova-docs | 1 | 1 | 0 | 0 |
| apache/camel-k | 1 | 0 | 1 | 0 |
| apache/fineract-backoffice-ui | 1 | 0 | 1 | 0 |
| apache/security-dash | 1 | 0 | 0 | 1 |
| mastra-ai/mastra | 1 | 0 | 0 | 1 |
| Whxuan0701/true-cost-chrome-extension | 1 | 0 | 1 | 0 |
| **Total** | **91** | **28** | **55** | **8** |

## Maintenance

PR 状态会随维护者审阅而变化。更新主页前，应重新运行 GitHub 作者检索，并只把 `MERGED` 项目计入“已合并成果”。
