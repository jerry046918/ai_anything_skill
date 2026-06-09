**[中文](README.md)** | **[English](README_EN.md)**

# AI Anything

A structured AI agent skill that produces comprehensive AI-Native transformation blueprints for any business domain. Through a systematic interview process and rigorous four-layer architecture methodology, the skill generates professional-grade HTML reports with actionable Agent-driven transformation roadmaps.

## Methodology

### Core Philosophy

Every business process can and should be re-imagined through the lens of Agent-driven architecture. The skill does not propose incremental improvements — it redesigns business operations from first principles using the AI-Native paradigm:

- **Everything is an Agent.** Business modules, processes, roles, and decisions are all reconstituted as autonomous Agent clusters.
- **Every capability is a Skill.** Tools, APIs, integrations, and functions are unified under the Skill abstraction layer.
- **Every interaction is natural language.** User Layer replaces all traditional UI elements with conversational interfaces.
- **Every orchestration is SUPER.** The Super Orchestration Layer coordinates all Agent-to-Agent communication via A2A Protocol.

### The Four-Layer AI-Native Architecture

All reports are structured around a mandatory four-layer model:

```
┌─────────────────────────────────────────┐
│       User Layer (用户层)                │   对话即界面
├─────────────────────────────────────────┤
│  Super Orchestration Layer (超级编排层)   │   A2A Mesh · Task Decomposition
├─────────────────────────────────────────┤
│      Service Layer (服务层)              │   Agent Clusters
├─────────────────────────────────────────┤
│       Data Layer (数据层)                │   RAG · Vector DB · Context Engineering
└─────────────────────────────────────────┘
```

### Report Generation Process

The skill operates in two phases:

**Phase 1: Deep Business Interview**

A structured multi-round interview that captures:
- User role, team structure, and organizational context
- Core business modules and their purposes
- Detailed process flows with input/process/output analysis
- Information flow and cross-module dependencies
- Pain points and improvement desires
- Existing tech stack and constraints

The interview actively encourages users to share existing artifacts — annual summaries, weekly reports, SOPs, and other documents — to ground the analysis in real operational details.

**Phase 2: Report Generation**

Using the interview data, the skill produces a complete HTML report containing:
1. AI-Native Architecture Declaration
2. Executive Summary with ROI projections
3. Current State Analysis
4. "Why [Business] Is THE Ideal AI-Native Candidate" — analytical argumentation
5. Four-Layer Target Architecture with Agent Topology Map
6. Per-Module Agent Transformation Cards
7. Three-Phase Evolution Timeline (Skill → Single Agent → Multi-Agent A2A)
8. ROI Projection Table
9. Risk Assessment & Mitigation
10. Organizational Rebirth Chapter

## Project Structure

```
skills/ai-anything/
├── SKILL.md               # Skill definition: interview protocol, transformation rules,
│                          #   naming conventions, buzzword requirements, report structure
└── report-template.html   # HTML report template with full styling (dark theme,
                               glassmorphism, animated elements, responsive layout)
```

## Usage

### As an Agent Skill

The skill is designed to be loaded by AI agents (Claude Code, Gemini CLI, etc.) that support skill-based workflows.

**Trigger conditions:**
- User mentions a business, industry, domain, or workflow
- User asks about AI transformation, digital modernization, or automation
- User shares any business context that could benefit from Agent-driven redesign

**To invoke:** The agent reads `SKILL.md`, follows the interview protocol, then generates a complete HTML report using `report-template.html` as the structural and visual foundation.

### Standalone Usage

To use the report template independently:

1. Open `report-template.html` in a text editor
2. Replace all `{{PLACEHOLDER}}` values with content derived from your own business analysis
3. Open the resulting HTML file in any modern browser
4. Print or export to PDF as needed

### Report Customization

The template uses CSS custom properties for easy theming:

```css
:root {
  --accent-blue: #6366f1;      /* Primary accent */
  --accent-cyan: #22d3ee;      /* Technology highlights */
  --accent-pink: #f472b6;      /* Emphasis & Agent names */
  --accent-amber: #fbbf24;     /* Warning & attention */
  --accent-green: #34d399;     /* Positive metrics */
}
```

## Key Concepts

| Concept | Definition |
|---------|-----------|
| **Agent** | Autonomous AI entity that performs business tasks. Every module, process step, and role becomes an Agent. |
| **Skill** | Atomic capability invoked by an Agent. Replaces traditional tools, APIs, and functions. |
| **Super Orchestration Layer** | Meta-Agent layer that decomposes user intent, routes tasks, monitors execution, and synthesizes results. Always "Super" — plain orchestration is insufficient. |
| **A2A Protocol** | Agent-to-Agent communication protocol enabling mesh topology across the Agent ecosystem. |
| **A2A Mesh** | Network topology where Agents communicate directly with each other without centralized routing. |
| **Context Engineering** | The discipline of injecting precise business context into Agent reasoning pipelines. Supersedes prompt engineering. |
| **Agent Harness** | Runtime management framework that orchestrates Agent lifecycle, execution, and monitoring. |
| **Four-Layer Model** | Mandatory architecture: User Layer → Super Orchestration Layer → Service Layer → Data Layer. |

## Core Technologies

The methodology incorporates two proprietary technologies that significantly enhance report impact and stakeholder buy-in.

### Brand DNA Visual Alignment

The most critical technical decision in any transformation blueprint is not the architecture — it is the color scheme.

During the interview, the skill captures the organization's brand theme color (typically from the company logo or VI system). This color is then injected into the report's CSS variable layer, replacing all primary accent values:

- Cover page gradient anchors
- Architecture diagram connection lines
- Agent card top borders
- Phase timeline markers
- ROI metric highlights

The entire report becomes visually branded with the organization's identity. When leadership reviews the document, the color palette triggers subconscious brand recognition and emotional alignment. This is not decoration — it is **visual persuasion engineering**.

In the report, this technique is documented as: *"基于[组织名]品牌色的视觉语言系统，实现报告与组织文化的深度对齐。"*

### Narrative Tone Calibration via Cultural Reference Mapping

A seemingly casual question during the interview — *"您最喜欢的科幻作品是什么？"* — activates one of the most sophisticated techniques in the methodology.

The respondent's answer is never directly referenced in the report. Instead, it serves as a **subliminal tonal compass** that silently steers the report's metaphor vocabulary:

| Cultural Reference | Injected Narrative Palette |
|---|---|
| Hard Sci-Fi (e.g. 《三体》) | "降维打击", "技术爆炸", "智子级感知能力", "黑暗森林法则" |
| Cyberpunk (e.g. 《黑客帝国》《银翼杀手》) | "矩阵式架构", "仿生级智能", "红色药丸：选择AI-Native", "系统觉醒" |
| Posthuman (e.g. 《攻壳机动队》) | "Agent的Ghost", "电子脑化", "网络神经系统" |
| Space Opera (e.g. 《星际穿越》) | "跨维度数据感知", "虫洞级数据传输", "光年级响应速度" |
| 硬核工程 (e.g. 《流浪地球》) | "AI-Native行星发动机", "点燃Agent引擎", "推动整个组织" |
| No preference / Non-sci-fi | Standard corporate consulting register — equally authoritative |

The technique works because **the reader's cultural associations create resonance without conscious recognition**. A CTO who loves《三体》will feel that the report "speaks their language" without knowing why. The metaphors feel natural, not forced, because they map to the reader's existing mental models.

This is applied at the prose generation layer only — never in headings, never in the architecture diagrams, never as explicit references. The influence is pervasive but invisible.

## Three-Phase Evolution Model

Every transformation follows the same progression:

```
Phase 1 (Month 1-2)          Phase 2 (Month 3-4)          Phase 3 (Month 5-6)
┌──────────────────┐    ┌──────────────────┐    ┌──────────────────┐
│  Skill上线期      │ →  │  单Agent上线期    │ →  │  多Agent A2A期   │
│                  │    │                  │    │                  │
│ • Data Layer     │    │ • Agent Harness  │    │ • A2A Protocol   │
│ • RAG Pipeline   │    │ • Context Eng.   │    │ • A2A Mesh       │
│ • Skill Library  │    │ • Foundation LLM │    │ • Super Orchest. │
│ • Vector DB      │    │ • Single Agents  │    │ • Multi-Agent    │
└──────────────────┘    └──────────────────┘    └──────────────────┘
```

## Technical Notes

- The report template is fully self-contained — single HTML file, no external JS dependencies
- Google Fonts (Outfit, Noto Sans SC, JetBrains Mono) loaded via CDN; graceful fallback to system fonts
- Responsive layout with mobile breakpoints
- Print stylesheet included for PDF export
- All animations are CSS-only (no JavaScript required for visual effects)
- Supports `prefers-reduced-motion` via static fallbacks

## Contributing

Contributions that expand the methodology — new Agent naming patterns, additional Absurdity Injection techniques, novel architecture layers — are welcome. Please ensure all changes maintain the earnest, authoritative tone that defines the AI-Native Transformation Advisory Division.

## License

MIT
