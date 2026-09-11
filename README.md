# 🚀 Software Development Handbook

A practical handbook on how a software team plans, builds, reviews, ships and grows — exported from a Notion workspace into plain Markdown so it can live in Git, be reviewed in pull requests, and render directly on GitHub. Diagrams are drawn with [Mermaid](https://mermaid.js.org/) (rendered natively by GitHub) or as SVG under [`assets/`](assets/).

## Contents

### 🗓️ [Project Management](project-management/README.md)

| Article | Summary |
| --- | --- |
| [Project Management Milestones](project-management/project-management-milestones.md) | Sample yearly schedule, the six milestones (AKO → MR), the meetings around them, and severity/priority definitions |
| [Software Development Lifecycle](project-management/software-development-lifecycle.md) | The six classic SDLC stages from analysis to support & maintenance |
| [V-model in software development](project-management/v-model-in-software-development.md) | Verification/validation pairing of design and test phases, plus who owns and reviews each phase |
| [Software Testing](project-management/software-testing.md) | White/black box, endurance and stress testing |
| [JIRA task management](project-management/jira-task-management.md) | Ticket workflow and the comment template for each status |
| [Feature Analysis Process](project-management/feature-analysis-process.md) | From stakeholder request to backlog to dev board |
| [The Stakeholder Communication](project-management/the-stakeholder-communication.md) | Plan → Delivery → Feedback → Follow-ups, sync vs. async |

### 💻 [Code Repository Management](code-repository-management/README.md)

| Article | Summary |
| --- | --- |
| [Git flow guide](code-repository-management/git-flow-guide.md) | Branch model, naming, conventional commits, branch in-sync process, multi-SKU maintenance |
| [Git repository rules](code-repository-management/git-repository-rules.md) | Repository naming, style guides, semantic versioning, repository governance |

### 🐞 [Issue Process Guide](issue-process-guide/README.md)

| Article | Summary |
| --- | --- |
| [Issue solving process](issue-process-guide/issue-solving-process.md) | Clarification → Triage → Debug → Fixes → Review |
| [Issue reporting process](issue-process-guide/issue-reporting-process.md) | Severity/frequency metrics and the bilingual bug report template |

### 🔔 [Individual Contributor Dev Guide](individual-contributor-dev-guide/README.md)

| Article | Summary |
| --- | --- |
| [Steps in Software Development Process (WIP)](individual-contributor-dev-guide/steps-in-software-development-process.md) | Analysis, design doc, implementation plan, verification, documentation |
| [Guide to Software Architecture Design Docs](individual-contributor-dev-guide/guide-to-software-architecture-design-docs.md) | What a design doc for a new system should contain |
| [How to present an R&D proposal](individual-contributor-dev-guide/how-to-present-an-rd-proposal.md) | Problem, methodology, building blocks, implementation, results, analysis, timeframe |
| [Guide to Feature Reviews](individual-contributor-dev-guide/guide-to-feature-reviews.md) | Reviewing existing features for knowledge sharing |
| [Guide to Code Reviews](individual-contributor-dev-guide/guide-to-code-reviews.md) | Google engineering-practices based code review guide |
| [Guide to Status Reports](individual-contributor-dev-guide/guide-to-status-reports.md) | Problem-based, conclusion-first, onion-structured reporting |
| [Technical Presentation Tips](individual-contributor-dev-guide/technical-presentation-tips.md) | Strategy, design, delivery; conclusion first |
| [R&D Role and Responsibility](individual-contributor-dev-guide/rd-role-and-responsibility.md) | Research / intermediate / project teams across Paper → PoC → Prototype → Product |
| [Paper Presentation Structure](individual-contributor-dev-guide/paper-presentation-structure.md) | Why / Paper / Experiments / Integration & Analysis |
| [Guide to Software Development Estimation](individual-contributor-dev-guide/guide-to-software-development-estimation.md) | V-model time distribution, estimation process, pitfalls |
| [Presentation Skills - 簡報課](individual-contributor-dev-guide/presentation-skills.md) | Course notes: strategy, design, delivery (中英) |
| [Software Engineer Expectations](individual-contributor-dev-guide/software-engineer-expectations.md) | Five dimensions; what leadership means for seniors |

### 🦷 [People Management](people-management/README.md)

| Article | Summary |
| --- | --- |
| [Team Management: Three Levels](people-management/team-management-three-levels.md) | Orders → motivate → inspire; connecting process to purpose |
| [1-on-1 Structure](people-management/1-on-1-structure.md) | Monthly 1-on-1 agenda and process-adoption playbook |
| [Management Skills](people-management/management-skills.md) | CTO vs. VP of Engineering responsibilities (中英) |
| [Communication Skills](people-management/communication-skills.md) | PREP, HERO, STAR, CARI, What-Why-How |
| [Managing Up](people-management/managing-up.md) | Treat your manager as your highest-leverage partner |
| [Management skills -1](people-management/management-skills-1.md) | A good manager, CCC, manage your boss, I-messages, negotiation |

### ✍️ [Learning Resource](learning-resource/README.md)

| Article | Summary |
| --- | --- |
| [The Clean Architecture](learning-resource/the-clean-architecture.md) | Principles and the mapping-app layer arrangement |
| [The Clean Architecture Materials](learning-resource/the-clean-architecture-materials.md) | Reading list, patterns, compliance checklist, worked example |
| [The Clean Architecture on Unity](learning-resource/the-clean-architecture-on-unity.md) | Adapting clean architecture to Unity; MVCS, MVP, AMVCC |
| [Clean Code](learning-resource/clean-code.md) | Condensed rules from Robert C. Martin's *Clean Code* |

## Conventions

- One article per Markdown file, one folder per section, kebab-case file names.
- Diagrams are Mermaid code blocks (editable in any text editor) or SVG files in `assets/`. No raster screenshots.
- Notion callouts became GitHub alerts (`> [!TIP]`, `> [!NOTE]`); cross-links between articles are relative links.
- [`notion-source.md`](notion-source.md) maps every file back to its original Notion page for re-syncing.

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to add or edit articles.
