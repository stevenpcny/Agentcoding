# X Programming Knowledge Base

## Purpose
把社交平台线索蒸馏成可供编程 agent 使用的工程规则、检索入口和证据卡片。

## Start here
- Agent entrypoint: `/Users/xxxxx/.hermes/x-knowledge/AGENT_README.md`
- Topic index: `/Users/xxxxx/.hermes/x-knowledge/knowledge/indexes/by-topic.md`
- Confidence index: `/Users/xxxxx/.hermes/x-knowledge/knowledge/indexes/by-confidence.md`
- Promotion candidates: `/Users/xxxxx/.hermes/x-knowledge/knowledge/indexes/promotion-candidates.md`
- Confidence rubric: `/Users/xxxxx/.hermes/x-knowledge/knowledge/standards/confidence-rubric.md`
- Note template: `/Users/xxxxx/.hermes/x-knowledge/knowledge/standards/note-template.md`

## Latest inputs
- 最新原始数据: `/Users/xxxxx/.hermes/x-knowledge/data/raw/x_bookmarks/bookmarks_20260516_120545.json`
- 最新分诊报告: `/Users/xxxxx/.hermes/x-knowledge/reports/triage_20260516_120545.md`
- 最新深化报告: `/Users/xxxxx/.hermes/x-knowledge/reports/deepening_20260516_round2.md`
- 指令审查报告: `/Users/xxxxx/.hermes/x-knowledge/reports/agent-instructions-review_20260516_120545.md`
- 重构方案: `/Users/xxxxx/.hermes/x-knowledge/reports/kb-restructure-proposal_20260516_083054.md`

## Primary playbooks

### agent-coding
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-coding/goal-and-task-framing.md`
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-coding/repo-instructions-and-project-memory.md`
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-coding/verification-and-review-loops.md`
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-coding/token-and-context-engineering.md`
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-coding/self-correction-and-recovery.md`
- umbrella: `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-coding/goal-driven-workflows.md`

### agent-infra
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-infra/skills-mcp-hooks-subagents.md`
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/agent-infra/multi-agent-orchestration.md`

### automation
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/automation/browser-to-api-and-native-tools.md`

### code-retrieval
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/code-retrieval/graph-retrieval-for-code.md`

### knowledge-systems
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/knowledge-systems/knowledge-pipeline-and-markdown-kb.md`

### business
- `/Users/xxxxx/.hermes/x-knowledge/knowledge/playbooks/business/agent-driven-business-workflows.md`

## Operating rules
- 先读最相关 playbook，再读 notes
- 尽量读具体 playbook，不要直接拿 umbrella 文件当全部上下文
- A/B/C 评级以 `knowledge/standards/confidence-rubric.md` 为准
- 社交帖默认是线索，不是最终工程定论
- business 类内容只作机会信号，不直接上升为工程规则

## Current improvement priorities
1. 逐条复核现有 A 级 notes
2. 给 notes 增加 frontmatter
3. 把过宽的 topic 桶继续拆细
4. 把 note 中的社交句式改写成工程句式
