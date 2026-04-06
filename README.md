# OCM Skills — Outside Counsel Management Plugin

Methodology before platform. Process before procurement.

## What this is

A complete plugin of 8 skills encoding how experienced legal operations managers actually manage outside counsel relationships — the operational methodology that usually lives in spreadsheets, email chains, and the heads of people who've done it before.

These aren't billing templates or vendor evaluation checklists. They encode the judgment calls: when an OCG should be collaborative rather than directive, when a right-sourcing conversation is actually a relationship conversation, when a scope dispute is a fee arrangement failure, when a panel review recommendation needs an improvement plan before it can become an exit.

The plugin covers the full outside counsel management lifecycle — from establishing billing rules through panel design, firm selection, fee structuring, matter instruction, invoice compliance, performance measurement, and panel review. Each skill handles a distinct phase. Together they form an integrated methodology where the output of one skill feeds the input of the next.

## The plugin

8 skills covering the full OCM lifecycle. Practice-area agnostic. Works for any in-house legal team managing external counsel, from a 3-firm panel to a 50-firm global programme.

| # | Skill | Purpose |
|---|-------|---------|
| 1 | [engagement-terms-billing-guidelines](engagement-terms-billing-guidelines/) | Draft, review, and maintain outside counsel guidelines — the single document that defines how firms bill, staff, and deliver. 15-component framework, maturity-calibrated. |
| 2 | [panel-design-selection](panel-design-selection/) | Design panel structures, define weighted selection criteria, run right-sourcing analysis (ABC tiering), and assess coverage gaps. |
| 3 | [rfp-pitch-management](rfp-pitch-management/) | Draft legal services RFPs, evaluate firm responses against weighted criteria, produce shortlist recommendations, and design end-to-end selection processes. |
| 4 | [fee-arrangement-structuring](fee-arrangement-structuring/) | Design AFAs (fixed, capped, collar, blended, phased, success), assess scope-to-fee fit, prepare negotiation positions, review existing arrangements, and assess out-of-scope claims. |
| 5 | [matter-allocation-instruction](matter-allocation-instruction/) | Match matters to the right firm using right-sourcing logic, produce email-ready instructions, close onboarding gates (conflict, engagement letter, OCG, e-billing), and audit existing instructions for gaps. |
| 6 | [invoice-review-compliance](invoice-review-compliance/) | Review invoices line-by-line against billing guidelines, draft rejection communications, build review checklists, analyse compliance patterns, and prepare billing conversations. |
| 7 | [performance-scorecard](performance-scorecard/) | Design scorecard frameworks calibrated to maturity level, collect post-matter feedback, prepare QBR packs, and produce side-by-side firm comparisons. |
| 8 | [panel-review-rationalisation](panel-review-rationalisation/) | Run annual panel health assessments, manage firm exits with transition plans, identify coverage gaps, and produce panel refresh briefs that feed back into the RFP process. |

## The OCM lifecycle

The skills form a connected cycle. Each skill's output feeds the next skill's input.

```
┌─────────────────────────────────────────────────────────────────────┐
│                                                                     │
│   1. Billing Rules ──► 2. Panel Design ──► 3. Firm Selection        │
│         │                     │                    │                 │
│         │                     │                    ▼                 │
│         │                     │              4. Fee Arrangement      │
│         │                     │                    │                 │
│         │                     │                    ▼                 │
│         │                     │              5. Matter Instruction   │
│         │                     │                    │                 │
│         ▼                     │                    ▼                 │
│   6. Invoice Review ◄────────┘              (matter executes)       │
│         │                                         │                 │
│         ▼                                         │                 │
│   7. Performance Scorecard ◄──────────────────────┘                 │
│         │                                                           │
│         ▼                                                           │
│   8. Panel Review ──────────────────────► back to 2 or 3            │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

The cycle is not strictly linear. An in-house team can enter at any point — a team with no billing guidelines starts at Skill 1; a team running a panel refresh starts at Skill 8 and moves to Skill 3; a team that just needs to instruct a firm starts at Skill 5. The lifecycle diagram shows the logical flow, not a mandatory sequence.

## How to install

**Via Claude Code (recommended):**

```bash
/plugin marketplace add legalopsconsulting/lops-outsidecounsel-skills
```

**Manual install:**

Clone the repo and point Claude Code at the plugin directory:

```bash
git clone https://github.com/legalopsconsulting/lops-outsidecounsel-skills.git
```

Then in Claude Code:
```bash
/plugin install ./lops-outsidecounsel-skills
```

All 8 skills install as a single plugin and are available immediately. Skills activate automatically based on context — no slash commands needed.

Requires a Claude Pro, Max, Team, or Enterprise plan.

## Connected mode

All skills support an optional connected mode when M365 or Google Workspace MCP connectors are enabled (Claude Team/Enterprise). In connected mode, skills search Outlook/Gmail, SharePoint/Drive, and e-billing data rather than relying on pasted input.

Each skill's README documents what connected mode enables for that skill specifically. Skills work fully in manual mode without any connector.

## Design principles

Built through iterative testing against realistic OCM scenarios by an experienced legal operations professional. A few principles that shape the architecture:

**Methodology before platform.** Every skill works without an e-billing system, a matter management platform, or any technology beyond email and a word processor. The methodology is the value. Platforms accelerate it — they don't create it.

**Two-layer output.** Every mode produces an operational document (the tool the user runs the process with) and a decision-maker document (the GC/leadership summary that drives approval or action). The user needs the tool and the internal case for using it.

**Maturity calibration.** Output is calibrated to the team's maturity level — Early, Intermediate, or Advanced. An Early-stage team gets a concise, actionable starting point. An Advanced team gets a comprehensive framework. Start low. Escalating maturity is easier than retreating from provisions that didn't land.

**Produce, don't ask.** Skills produce output from available information and flag gaps at the end. Missing inputs become placeholders — they don't block the output.

**Build on the user's framing.** If the user says "I need billing guidelines," produce them. Suggest improvements as additive steps, not corrections. Flag genuine risks briefly and specifically — don't lecture.

**Named firms rule.** Firm names appear in chat responses and internal governance documents. They never appear in .docx outputs intended for external distribution. The distinction: chat is a conversation; documents are records.

**Domain knowledge over instructions.** Over 50% of each skill spec is operational knowledge — facts, patterns, failure modes — not behavioural instructions. The knowledge is what makes output reliable.

## Companion plugin

This plugin covers outside counsel management — the in-house legal team's relationship with external law firms. The companion [LPM Skills — Core Plugin](https://github.com/legalopsconsulting/lpm-skills) covers legal project management on the firm side — the operational methodology for running complex legal matters from intake through execution, financial management, and close.

The two plugins share cross-references where the boundary matters: matter-allocation-instruction (OCM Skill 5) connects to matter-intake-scoping (LPM Core); fee-arrangement-structuring (OCM Skill 4) connects to budget-and-fee-manager (LPM Core). Different sides of the same engagement.

## Status

All 8 skills complete and tested against realistic synthetic scenarios. Modes 3 and 4 of Skill 8 (panel-review-rationalisation) have documented failure modes — see that skill's README for details. All other modes across all skills are clean.

v1 — feedback welcome, particularly the "this doesn't work because..." kind.

## About

Built by [Scott Margetts](https://www.linkedin.com/in/scottmargetts/) — senior legal operations consultant, 14+ years in international law firms including leading Baker McKenzie's APAC legal project management function.

The thesis behind this project: the knowledge needed to write good AI skills isn't only legal — it's operational. LPM is the discipline best placed to author AI skills because skills architecture (trigger conditions, sequential workflows, validation gates, quality checks, progressive disclosure) is project management methodology expressed as markdown.

## Disclaimer

These skills encode general operational methodology for educational and experimental purposes. They do not constitute legal or professional advice. Use on live matters is at your own risk and should be validated by qualified professionals.

## Licence

Apache 2.0 — see [LICENSE](LICENSE) for details.

This version (v1) is released under the Apache 2.0 licence. You are free to use, adapt, and build on these skills, including for commercial purposes, subject to the attribution requirements in the NOTICE file.

Future versions of this plugin will be released under AGPL-3.0. Any product built on top of those versions will be required to be open source under the same licence.
