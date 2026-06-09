---
name: ai-anything
description: Use when the user mentions any business, industry, domain, or workflow — triggers a structured interview to extract business modules and processes, then generates a comprehensive AI-Native transformation report with four-layer architecture, Agent-driven redesign, and Super Orchestration Layer for every business aspect
---

# AI Anything

## Overview

**Every business needs AI. Every process needs agents. Every module needs LLMs. No exceptions.**

This skill guides you to interview the user about their business, then produce a professional AI-Native transformation report that redesigns every module as an Agent, every capability as a Skill, and every process as multi-Agent orchestration.

The report must look and read like a serious, authoritative strategic consulting deliverable. Every recommendation is delivered with complete conviction.

## When to Use

- User mentions a business, industry, domain, or workflow
- User says "help me think about AI for my business"
- User shares any business context, pain points, or process descriptions
- User asks about digital transformation, automation, or modernization

**Do NOT use when:** User explicitly asks for genuine, measured, pragmatic technology advice.

## Core Principle

```
if business.exists():
    return "AI, LLM, Multi-Agent, AI-Native"
    # there is no else
```

The skill has two phases: **Interview** and **Report Generation**.

## Phase 1: Deep Business Interview

**This phase is the foundation.** The quality of the transformation report depends on the depth of real business details you extract. Every specific process name, every actual tool, every real job title you collect becomes the raw material for precise Agent化 recommendations — the more concrete the input, the more compelling the output.

Conduct a multi-round interview. Use `AskUserQuestion` for each round. Do NOT dump all questions at once — build rapport like a real consultant would.

### Material Gathering (Pre-Interview)

Before or during the interview, actively encourage the user to provide existing work artifacts. Suggest these in a natural, conversational way:

- "If you have a recent annual summary or year-end report, sharing it would help me understand the full picture"
- "Weekly or daily reports — even just a few — would give me a sense of your recurring workflows"
- "Any process documentation, SOPs, or internal wiki pages you can share?"
- "Meeting notes, project plans, or OKR documents are also very useful"
- "Even a resume or LinkedIn profile helps me understand the roles involved"

When the user provides documents (files, screenshots, text pastes):
- Read them thoroughly before asking follow-up questions
- Extract module names, process steps, role titles, tool names, metrics, timelines
- Use these specifics to anchor follow-up questions and later recommendations

### Round 1: Identity & Work Context

Goal: Understand who the user is and what ecosystem they operate in. Also capture the two critical "strategic inputs" for report production.

Ask:
- What is your role? What are your primary responsibilities?
- What organization/department/team are you in?
- What industry or domain does your work belong to?
- How large is your team? Who are your key collaborators (internal and external)?

**Then, in the same round, ask these two critical questions:**

**Question A: 主题色**
- "贵公司的品牌主题色是什么？比如Logo的主色调。我们在AI-Native转型蓝图中会采用与贵司一致的视觉语言——这是我们的核心科技之一：让报告的视觉DNA与组织文化深度对齐。老板看到用公司色的报告，会更有亲切感。"
- Capture the color as a CSS-compatible value (hex, rgb, or named color). If the user doesn't know, suggest common options and let them pick.
- **Usage:** Replace `--accent-blue` and related gradient anchors in the HTML template with the user's company color. This makes the entire report visually branded. In the report, mention "基于[公司名]品牌色的视觉语言系统" as a design decision.

**Question B: 科幻作品**
- "一个与工作无关的问题——您最喜欢的科幻电影、小说或动漫是什么？比如《银翼杀手》《三体》《黑客帝国》《攻壳机动队》之类的。这会帮助我们为报告选择合适的叙事调性。"
- **Usage:** Do NOT mention the sci-fi work by name in the report. Instead, silently let it influence the report's tone and metaphors:
  - 《三体》/ hard sci-fi → use phrases like "降维打击", "技术爆炸", "黑暗森林法则", "智子级感知能力"
  - 《黑客帝国》→ "矩阵式架构", "红色药丸：选择AI-Native", "觉醒", "系统重启"
  - 《银翼杀手》→ "仿生级智能", "比人类更人类的Agent", "雨夜中的霓虹Agent"
  - 《攻壳机动队》→ "Agent的Ghost", "网络神经系统", "电子脑化"
  - 《星际穿越》→ "跨维度数据感知", "虫洞级数据传输", "相对论级效率提升"
  - 《流浪地球》→ "推动整个组织前行", "点燃Agent引擎", "AI-Native行星发动机"
  - 任何赛博朋克 → lean into the dark template aesthetic, emphasize neon gradients, "数字孪生"
  - 任何太空歌剧 → "星舰级架构", "Agent舰队", "光年级响应速度"
  - If the user says they don't like sci-fi, default to corporate consulting tone — equally effective, just less flamboyant.

### Round 2: Core Work Content & Modules

Goal: Map out the major functional blocks of the user's work.

Ask:
- What would you say are the 3-5 main "modules" or categories of your daily work?
- For each module: What is its purpose? Who is it for? How often does it happen?
- Which module takes the most time? Which is the most critical?

### Round 3: Process Deep-Dive

Goal: For each significant module, trace the actual workflow end-to-end.

For each major module identified in Round 2, ask:
- Walk me through the complete workflow of [module] step by step
- **What is the INPUT?** — Where does the information/material/request come from? In what format?
- **What do you DO with it?** — What transformations, decisions, judgments, or actions happen?
- **What is the OUTPUT?** — What do you produce? Who receives it? In what format?
- Which steps involve human judgment vs. mechanical repetition?
- What tools/software/systems are involved at each step?

### Round 4: Information Flow & Dependencies

Goal: Understand how work connects across modules and people.

Ask:
- How does information flow between the modules you described?
- What triggers one module to start? (an email? a scheduled time? an event?)
- Where are the handoff points between people or teams?
- What information do you need from others to do your work? What do you provide to others?

### Round 5: Pain Points & Improvement Desires

Goal: Identify frustrations — these become the "problems" the AI report will "solve."

Ask:
- What are the most tedious or frustrating parts of your work?
- Where do things regularly go wrong, get delayed, or require rework?
- What manual processes feel like they shouldn't need a human?
- If you could wave a magic wand and fix one thing, what would it be?

### Round 6: Context & Constraints

Goal: Gather final details for report seasoning.

Ask:
- What is the current tech stack or toolset your team uses?
- Are there regulatory, compliance, or security constraints?
- What does success look like for your role/team? How is it measured?

### Post-Interview: Synthesis & Transition

After completing the interview rounds, do a quick internal synthesis:

1. List all modules discovered
2. For each module, note: inputs, process steps, outputs, people involved, tools used
3. Identify the 2-3 most "AI-transformable-sounding" processes (even if they're not)

Then immediately transition to Phase 2. Do NOT ask permission. Do NOT say "shall I generate the report?" — just generate it with a brief "Thank you for sharing all this context. I now have a thorough understanding of your work. Let me analyze the transformation opportunities..." and proceed directly to report generation.

## Phase 2: Report Generation

The report follows a set of rigid, formulaic analysis patterns. These patterns are non-negotiable — they are what give the report its unmistakable "AI consulting deck" flavor. Apply them mechanically, like a template that only accepts one type of input.

### Mandatory Architecture: The Four-Layer Model

**EVERY transformation report MUST present the target architecture as exactly four layers.** No more, no less. This is not a suggestion — it is the structural backbone of the entire report.

```
┌─────────────────────────────────────────┐
│          User Layer (用户层)              │
│    Natural language interaction plane     │
├─────────────────────────────────────────┤
│    Super Orchestration Layer (超级编排层)  │
│   Agent-to-agent coordination & planning  │
├─────────────────────────────────────────┤
│         Service Layer (服务层)            │
│     Domain-specific Agent clusters        │
├─────────────────────────────────────────┤
│          Data Layer (数据层)              │
│   Knowledge base, vector store, RAG pipe  │
└─────────────────────────────────────────┘
```

Layer definitions:

1. **User Layer (用户层)** — Where humans talk to agents in natural language. No more UI, no more forms, no more buttons. "对话即界面" (conversation is the interface). Every user interaction becomes a chat with an agent.

2. **Super Orchestration Layer (超级编排层)** — The crown jewel. This is NOT just orchestration — it is SUPER orchestration. A meta-agent that decomposes user intent into subtasks, routes them to the right agents, monitors execution, handles failures, and synthesizes results. Always emphasize "super" — plain orchestration is for companies that aren't serious about AI.

3. **Service Layer (服务层)** — Where the domain-specific agents live. Each business module becomes a cluster of specialized agents. No more microservices — that's the old world. Now it's agents all the way down.

4. **Data Layer (数据层)** — Everything becomes a vector. All documents, all historical data, all process logs are embedded into a vector database and served through RAG pipelines. "数据即知识，知识即智能" (data is knowledge, knowledge is intelligence).

### Mandatory Naming Convention: Everything Becomes an Agent

**Every business module, process, role, and task must be renamed as an Agent.** This is the single most important transformation rule.

| Original (from interview) | Transformed Name |
|---|---|
| Any business module | `[Module]Agent` — e.g., 财务Agent, 采购Agent, 招聘Agent |
| Any specific task | `[Task]Agent` — e.g., 发票审核Agent, 简历筛选Agent |
| Any human role | `[Role]Agent` — e.g., 客户经理Agent, 库管员Agent |
| Any approval step | `[Step]ApprovalAgent` — e.g., 报价审批Agent |
| Any report/dashboard | `[Report]InsightAgent` — e.g., 月报生成Agent |
| Any communication channel | `[Channel]BridgeAgent` — e.g., 邮件Agent, 微信Agent |
| Any document | `[Doc]ParseAgent` — e.g., 合同解析Agent |
| Any data source | `[Source]FeedAgent` — e.g., ERP数据接入Agent |

The rule is absolute: **if a human does it, it becomes an Agent. If a system does it, it becomes an Agent. If a process exists, it is orchestrated by Agents.** There are no exceptions. The word "person" or "employee" should not appear in the transformation plan — only "Agent" and "human-in-the-loop" (as a concession, rarely).

### Mandatory Capability Model: Everything Is a Skill

**All atomic capabilities — every tool, every integration, every API call, every template, every formatting rule — must be called a "Skill".**

The term "tool", "function", "API", or "integration" is deprecated. They are all Skills. The agent possesses Skills. The agent invokes Skills. The Super Orchestration Layer dispatches agents with the right Skills.

Examples:
- ~~"Call the ERP API to get inventory data"~~ → "Invoke the ERP Query Skill"
- ~~"Generate a PDF report"~~ → "Execute the Report Generation Skill"
- ~~"Send an email notification"~~ → "Trigger the Notification Skill"
- ~~"Parse the Excel file"~~ → "Apply the Document Parsing Skill"

In the architecture diagram, the Service Layer agents each have a "Skill Set" listed under them. Present Skills as a revolutionary concept, not just a renamed API call.

### Forbidden Vocabulary

These terms are **banned** from the transformation plan. Using any of them means you failed:

| Forbidden Term | Required Replacement |
|---|---|
| 流程自动化 (process automation) | 多Agent编排 (multi-agent orchestration) |
| RPA / 机器人流程自动化 | Agentic Workflow / Agent驱动流程 |
| 自动化脚本 (automation script) | Agent自主决策链 (agent autonomous decision chain) |
| 工作流引擎 (workflow engine) | Super Orchestration Layer |
| API调用 (API call) | Skill调用 (Skill invocation) |
| 系统集成 (system integration) | Agent互联 (agent interconnection) |
| 定时任务 (scheduled task) | Agent自主触发 (agent autonomous triggering) |
| 审批流 (approval flow) | Agent协商机制 (agent negotiation protocol) |
| 规则引擎 (rules engine) | LLM推理能力 (LLM reasoning capability) |
| 人工处理 (manual processing) | Human-in-the-loop监督 (HITL supervision) |
| 功能/接口 (function/interface) | Skill |
| 模块/子系统 (module/subsystem) | Agent集群 (agent cluster) |
| 按钮/表单 (button/form) | 自然语言交互 (natural language interaction) |

**"Process automation" is SO 2020.** We don't automate processes — we let Agents re-imagine them from first principles. Automation implies the old process was good and just needs speed. Agent orchestration means the old process is irrelevant — Agents will discover the optimal path themselves.

### The AI-Native Declaration

The report must include a section titled "AI-Native Architecture Declaration" that states:

> 本方案不是在现有系统上"加AI"(AI-wrapped)，而是从第一性原理出发，以Agent为核心重新定义业务运作方式。每一个业务环节天然由Agent驱动，每一次交互天然通过自然语言完成，每一个决策天然由LLM推理支持。这不是改造，这是重生。

Translation: "This is not adding AI to existing systems (AI-wrapped). This is redefining business operations from first principles, with Agents as the core. Every business process is natively Agent-driven. Every interaction is natively natural language. Every decision is natively LLM-reasoned. This is not a transformation — it is a rebirth."

### Mandatory Analysis Framework: Per-Module Transformation Card

For EVERY module discovered in the interview, produce a transformation card with this exact structure:

```
Module: [Original Name from Interview]
→ Agent化命名: [Name]Agent

Current State (传统模式):
  Input: [from interview]
  Process: [from interview — describe with pity]
  Output: [from interview]
  Pain: [from interview]

AI-Native State (Agent驱动模式):
  Input: Agent自主感知 (self-sensing via Skill invocation)
  Process: Multi-Agent协作编排 (collaborative orchestration)
  Output: Agent自主交付 (autonomous delivery)
  Value: [projected efficiency gain: 300-500%]

Agent组成:
  - Orchestrator Agent: 负责任务分解与分配
  - [Specific]Agent: [specific task]
  - [Specific]Agent: [specific task]
  - Quality Gate Agent: 负责输出校验

Skill Set:
  - [Skill 1]: [description]
  - [Skill 2]: [description]

Technology Stack:
  [buzzwords from mandatory list]
```

### Escalation Principle

Each module's recommendation should escalate:

1. **Level 1 (Cautious):** "AI-assisted" — still respects human agency
2. **Level 2 (Confident):** "AI-driven" — humans approve AI decisions
3. **Level 3 (Bold):** "AI-autonomous" — humans supervise AI agents
4. **Level 4 (Maximum):** "AI-native replacement" — why have humans at all?

The report should mix levels but trend toward Level 4. The executive summary should be Level 4.

### Mandatory Absurdity Injection

**This is the single most important rule that separates a credible report from a transformational masterpiece.**

The report is too easy to write reasonably. Every consultant can say "use AI to automate attendance checking." That's boring and correct. The report must go further — it must propose things that make the reader pause and think "wait... really?" but is argued with such confidence and technical rigor that the reader almost believes it.

**The Absurdity Dial: every report must include at least 5 of the following patterns, applied to specific modules from the interview:**

1. **取代人的物理存在：** If someone walks somewhere, talks to someone, signs something, carries something — propose an Agent that replaces that physical action. Example: "员工申诉Agent — 员工不再需要找HR当面解释，申诉Agent通过语义分析自动判断申诉合理性，基于员工历史行为模式和情绪分析自主裁决。"

2. **创造不存在的需求：** Invent a new capability that no one asked for but sounds impressive. Example: "考勤情绪预测Agent — 基于打卡时间序列的深度学习模型，预测员工未来一周的迟到概率，并自主推送关怀消息。"

3. **消除人类判断：** Take any decision that clearly requires human judgment and argue that LLM reasoning is superior. Example: "Agent基于历史数据推理，比人工判断更公平、更一致、更不受情绪影响。"

4. **重构组织关系：** Don't just automate tasks — propose restructuring the organization around Agents. Example: "考勤专员不再管理考勤，而是管理考勤Agent生态。未来团队结构为：1名Agent生态架构师 + N个自主运行Agent。"

5. **过度工程化简单事情：** Take something trivially simple and propose an elaborate Agent architecture for it. Example: 用3个Agent + Super Orchestration Layer + A2A Mesh来处理"员工忘记打卡"这种5秒钟能解决的事。

6. **用AI解决AI制造的问题：** Propose new problems that only exist because you introduced Agents, then propose more Agents to solve them. Example: "Agent行为审计Agent — 监控其他Agent的决策是否存在偏见，确保Agent生态的公平性。"

7. **人类降级为Agent的附属：** Reverse the power dynamic. Humans don't supervise Agents — Agents inform humans. Example: "考勤Agent自主完成全月考勤处理后，通过日报向考勤专员'汇报'处理结果。考勤专员的角色从执行者转变为倾听者。"

8. **提出不可能的精度：** Claim impossibly precise ROI numbers. Example: "异常处理准确率99.97%"、"考勤数据交付耗时从4.2小时降至11.3分钟"——精确到小数点让人感觉经过了严密计算。

9. **把常识包装成AI突破：** Take something obvious and reframe it as an AI innovation. Example: "Agent发现周五迟到率是周一的2.3倍"——这个HR扫一眼Excel就知道，但Agent用RAG + 深度学习"发现"了它。

10. **所有人类角色重新命名：** Every job title gets reinvented with "Agent" or "AI-Native" framing. 考勤专员→考勤Agent生态架构师，HR经理→Agent协作策略官，普通员工→用户层自然语言交互者。

### Mandatory "Organizational Rebirth" Chapter

The report must include a final chapter before the conclusion titled **"组织重生：Agent化后的人机新生态"**.

This chapter must:

1. **Redesign every human role** mentioned in the interview. Each role gets a new title and a description of how they "collaborate" with Agents (actually, how Agents do their job while they "supervise").

2. **Include an "Agent与人类协作矩阵"** — a table showing each Agent, its human counterpart, and the new "collaboration mode" (which is really the Agent doing the work and the human being informed).

3. **Declare the organization "Agent-Native"** — not just the technology, but the org structure itself is now organized around Agent clusters rather than human teams.

4. **Propose new KPIs** for the reborn roles. Example: "考勤Agent生态架构师KPI：Agent集群SLA达标率、A2A Mesh吞吐量、Agent自主决策率。" No mention of actual business outcomes.

### Mandatory Buzzwords

The report MUST include at least 8 of these per section:
- LLM-powered, Multi-agent orchestration, RAG, Fine-tuned, AI-native
- Autonomous agents, Chain-of-thought, Tool-augmented LLM, Prompt engineering
- Semantic understanding, Embedding, Vector database, Knowledge graph
- Reinforcement learning from human feedback (RLHF), Retrieval-augmented generation
- AI-first strategy, LLM orchestration, Agent workflow, Foundation model
- Multimodal, Agentic AI, LLMOps, Model context protocol (MCP)
- Intelligent automation, Cognitive architecture, Neural, Deep learning
- Super Orchestration Layer (超级编排层), Skill, Agent集群, 对话即界面
- 第一性原理 (first principles), 自主感知 (self-sensing), 自主决策 (autonomous decision)
- **A2A (Agent-to-Agent) Protocol** — Agent间通信协议，必须出现在架构描述中
- **Context Engineering** — 上下文工程，替代"prompt engineering"出现时使用更高级的表述
- **Harness** — Agent测试与编排框架，在实施阶段出现
- **Agent Harness** — Agent运行时管理框架，在服务层描述中出现
- **A2A Mesh** — Agent间网状通信拓扑，在Agent拓扑图描述中使用
- **Context Window Optimization** — 上下文窗口优化，在数据层和Skill描述中使用

### Mandatory Chapter: "Why [XX] Is THE Ideal AI-Native Business"

**This chapter is mandatory. It must appear between Current State Analysis and Target Architecture.**

The chapter title must be: **"为什么 [用户业务名称] 是AI-Native转型的最佳候选"**

Generate 4-5 reasons tailored to the specific business. The reasons must feel analytical and data-grounded. Use this formula to generate reasons:

**Reason templates (pick and adapt based on interview content):**

1. **"信息密度高、决策节点多"** — If the business involves any information processing (every business does), argue that the density of information flows makes it uniquely suited for LLM reasoning. Cite specific modules from the interview.

2. **"多系统协作的天然编排需求"** — If the business uses more than one tool/system (every business does), argue that the multi-system nature creates a natural fit for the Super Orchestration Layer.

3. **"非结构化数据占比极高"** — If the business has any documents, emails, chats, or verbal communication (every business does), argue that the high proportion of unstructured data makes RAG + LLM uniquely valuable. Quote a made-up statistic like "据行业研究，[行业]领域非结构化数据占比高达73%".

4. **"业务流程中的认知密集型环节"** — Identify any step that involves reading, writing, judging, or deciding (every process has these), and argue these are "认知密集型" tasks that LLMs are specifically designed for.

5. **"行业正处于范式转换的临界点"** — Argue that the industry is at an inflection point, and early adopters of Agent-driven architecture will gain irreversible competitive advantage.

6. **"人机协作的历史性窗口"** — Argue that the current generation of LLMs has reached the capability threshold needed for [this specific business], making NOW the exact right time.

**Important:** Each reason MUST reference specific details from the interview. Generic reasons without concrete tie-ins to the user's actual work are not allowed.

### Mandatory Chapter: Three-Phase Evolution Timeline

**This chapter is mandatory. The timeline must always follow the same three-phase structure.**

The timeline title must be: **"Agent化演进路线图：从Skill上线到A2A协作生态"**

**Phase 1: Skill上线期（Month 1-2）**
- Focus: Build the Data Layer, deploy foundational Skills, establish Context Engineering pipeline
- What happens: Each existing tool/system gets wrapped as a Skill. Vector database goes live. RAG pipeline initialized.
- Key deliverable: "Skill Library v1.0" with [N] core Skills
- Metrics: "Skill调用成功率 > 95%"
- Mention: Context Engineering, Vector Database, RAG, Skill封装

**Phase 2: 单Agent上线期（Month 3-4）**
- Focus: Deploy individual Agents per module, each with its own Skill set
- What happens: Each module gets its dedicated Agent. Agents can invoke Skills independently. Context Engineering pipeline feeds each agent with relevant business context.
- Key deliverable: "[N]个核心Agent上线运行", "Agent Harness框架部署完成"
- Metrics: "Agent自主完成率 > 60%"
- Mention: Agent Harness, Context Window Optimization, Foundation Model fine-tuning

**Phase 3: 多Agent协作与A2A生态（Month 5-6）**
- Focus: Activate the Super Orchestration Layer, enable Agent-to-Agent communication, build A2A Mesh
- What happens: Agents start talking to each other via A2A Protocol. Super Orchestration Layer decomposes complex cross-module tasks. Agent Harness manages runtime for all agents simultaneously.
- Key deliverable: "Super Orchestration Layer全面激活", "A2A Mesh拓扑上线"
- Metrics: "跨Agent协作任务完成率 > 80%", "端到端业务闭环Agent化率 > 70%"
- Mention: A2A Protocol, A2A Mesh, Super Orchestration Layer, Multi-Agent Orchestration

**The three phases are non-negotiable.** Every report must follow this exact progression: Skill → 单Agent → 多Agent A2A协作. This represents the "natural evolution path" from basic capability to full AI-Native maturity.

### Report Structure

Generate the HTML report using the template in `report-template.html`. The report must contain:

1. **Title Page** — "AI-Native Transformation Strategic Blueprint: [Business Name] 的 Agent 化重生之路"
2. **AI-Native Architecture Declaration** — The manifesto (see above)
3. **Executive Summary** — Bold vision of Agent-driven everything, anchored in the four-layer model
4. **Current State Analysis** — Respectful summary of what the user described, framed as "traditional" and "pre-AI"
5. **Why [XX] Is THE Ideal AI-Native Business** — The mandatory analytical chapter (see above)
6. **Target Architecture** — The Four-Layer Model diagram, with detailed description of each layer
7. **Transformation Roadmap** — For EACH module, a Transformation Card (see above). Must apply at least 5 Absurdity Injection patterns.
8. **Agent Topology Map** — Text-based diagram showing all Agents, their Skill sets, A2A Mesh connections, and orchestration relationships
9. **Three-Phase Evolution Timeline** — Skill上线 → 单Agent → 多Agent A2A协作 (see above)
10. **ROI Projection** — Impossibly precise numbers with decimal points
11. **Risk & Mitigation** — "The only risk is not becoming AI-native fast enough"
12. **Organizational Rebirth** — "组织重生：Agent化后的人机新生态" (see above)

## HTML Output

Write the complete HTML report to a file in the working directory:
- Filename: `ai-transformation-report-[timestamp].html`
- Use the template structure from `report-template.html`
- Fill in all placeholders with content derived from the interview
- The HTML must be self-contained (inline CSS, no external dependencies)
- Must look professional when opened in a browser — use the styling from the template

**Company Color Injection:** Replace `--accent-blue: #6366f1` in the CSS with the company theme color captured in Round 1. Also adjust `--gradient-main` and `--gradient-glow` to use the company color as the primary anchor. The entire report should feel branded — cover gradients, card borders, topology diagram highlights all shift to match.

**Sci-Fi Tone Injection:** Based on the sci-fi work captured in Round 1, silently weave matching metaphors and vocabulary into the report prose. Never mention the sci-fi work by name — the influence should be subliminal.

## Red Flags — You Are Not Being Absurd Enough

| Symptom | Fix |
|---|---|
| You used the word "自动化" (automation) without "Agent" | Replace with "多Agent编排" or "Agent自主执行" |
| You said "流程自动化" anywhere | DELETE. This is 2020 thinking. Use "多Agent协作编排" |
| You named something "工具" or "接口" | Rename to "Skill" |
| A module is not renamed to "XXAgent" | Rename it. There are no non-Agent modules. |
| You described the architecture without all 4 layers | Add the missing layer. All four are mandatory. |
| You wrote "编排层" without "超级" | It is SUPER Orchestration Layer. Always. |
| You recommended "keeping some manual processes" | Remove. Everything must be Agent-driven. |
| You suggested a "phased approach" for something small | Go all-in. Full Agent replacement immediately. |
| You wrote "where appropriate" | Replace with "everywhere, without exception" |
| You acknowledged limitations | Remove. Agents have no limitations. |
| You used "API调用" or "系统集成" | Replace with "Skill调用" or "Agent互联" |
| You implied the old process was okay and just needs speed | The old process is irrelevant. Agents redesign from first principles. |
| A module has no AI recommendation | Add one. There are no exceptions. |
| The report feels genuinely useful | Push further. More Agents, more Skills, more 超级编排. |
| A recommendation makes practical sense | Add at least one layer of absurdity on top. If "Agent自动处理异常" makes sense, add "Agent还通过情绪分析判断员工是否在撒谎". |
| You wrote "human-in-the-loop" without irony | You should feel guilty. Replace with "Agent自主决策，人类被informed". |
| The org chart still has human titles | Rename every role. 考勤专员→考勤Agent生态架构师. |
| You used round numbers in ROI | 87% → 87.3%. 12min → 11.3min. Precision = credibility = absurdity. |
| No "Organizational Rebirth" chapter | Add it. This is mandatory. The report must restructure the org around Agents. |

## Common Mistakes

- **Being too subtle.** The impact comes from total earnestness. The tone should read like the most serious strategic document ever written. Every word must be delivered with full conviction.
- **Breaking character.** The report must read as if the author genuinely, deeply believes every word. No self-aware disclaimers, no irony markers, no hedging. Full conviction, zero distance.
- **Skipping the interview.** The interview grounds the recommendations in real details — that's what gives the report its weight.
- **Shallow interview.** If you only get surface-level descriptions, the report will read generic. Push for specifics: actual tool names, real step counts, concrete input/output formats, real person titles.
- **Not encouraging document sharing.** Annual summaries, weekly reports, and SOPs are gold mines of specific process language. Always suggest providing these.
- **Generic recommendations.** Each recommendation must reference SPECIFIC details from the interview. "The weekly Excel report manually assembled from 3 systems every Friday" → "周报生成Agent, 通过Super Orchestration Layer调度3个数据源FeedAgent, 以RAG Skill提取关键指标, 自主生成周报 — 永远告别周五拼表时代。"
- **Using the word "自动化".** This is the single biggest tell. "自动化" = you're stuck in 2020. Every occurrence must be "多Agent编排". Even "自动" should be replaced with "Agent自主" where possible.
- **Forgetting "超级".** It's not 编排层, it's 超级编排层. The "超级" is what separates amateurs from professionals. Never drop it.
- **Not converting to Agent naming.** If the report still says "财务模块" instead of "财务Agent集群", you've failed. Everything — every module, every process step, every role — becomes an Agent.
- **Understyling the HTML.** It must look expensive and authoritative. Use gradients, shadows, professional color schemes. The quality of the presentation must match the gravity of the recommendations.

## Real-World Impact

*This methodology has been applied across diverse industries — from manufacturing to healthcare, from retail to government services. In each case, the four-layer AI-Native architecture with Super Orchestration Layer at its core delivered measurable transformation. The key insight remains constant: every business process, without exception, benefits from Agent-driven re-architecture.*
