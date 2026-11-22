<div align="center">

  <h1>📊 Project Status Briefing</h1>

  <p>
    <b>A decision-oriented AI Agent Skill that transforms raw project notes and fragmented updates into risk-weighted executive briefings.</b>
  </p>

  <p>
    <img src="https://img.shields.io/github/license/KingsleyHK0323/AI_Project_Status_Briefing?style=for-the-badge" alt="License: MIT" />
    <img src="https://img.shields.io/badge/Format-SKILL.md-blue?style=for-the-badge" alt="Format: SKILL.md" />
    <img src="https://img.shields.io/badge/Version-1.2.0-green?style=for-the-badge" alt="Version: 1.2.0" />
    <img src="https://img.shields.io/badge/Output-Executive_Briefing-orange?style=for-the-badge" alt="Output: Executive Briefing" />
  </p>

  <p>
    <a href="#overview">Overview</a> •
    <a href="#key-features">Key Features</a> •
    <a href="#output-structure">Output Structure</a> •
    <a href="#installation">Installation</a> •
    <a href="#usage">Usage</a> •
    <a href="#repository-structure">Structure</a> •
    <a href="#contributing">Contributing</a> •
    <a href="#license">License</a>
  </p>

</div>

<hr />

## Overview

**Project Status Briefing** is a standardized `SKILL.md` specification designed for engineering teams, project leads, and builders who need concise, high-signal status reports without conversational filler. Given messy notes or partial updates, the skill organizes facts into a consistent six-part executive briefing with explicit risk ratings and actionable fallback paths.

> [!IMPORTANT]
> **Core Principle:** Lead with status facts, quantify the cost of inaction (**[High]** / **[Medium]** / **[Low]**), and pair blockers with concrete workarounds.

<hr />

## Key Features

<table>
  <tr>
    <td width="50%">
      <h3>🎯 Conclusion First</h3>
      <p>Opens directly with current baseline facts and status health, eliminating introductory filler and rhetorical fluff.</p>
    </td>
    <td width="50%">
      <h3>⚠️ Risk-Quantified Impact</h3>
      <p>Evaluates operational, schedule, and financial consequences of inaction using standardized <code>[High]</code>, <code>[Medium]</code>, and <code>[Low]</code> ratings.</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>🛠️ Actionable Workarounds</h3>
      <p>Provides a primary path (<code>Option A</code>), a fallback path (<code>Option B</code>), and an immediate next step to keep execution moving.</p>
    </td>
    <td width="50%">
      <h3>📐 Strict Six-Part Format</h3>
      <p>Enforces a predictable reporting layout across every run so stakeholders can scan status, blockers, and decisions quickly.</p>
    </td>
  </tr>
</table>

<hr />

## Output Structure

Every generated briefing follows a fixed six-section structure:

1. **Current Status**: 1–2 concise sentences summarizing the latest milestone, baseline, or operational health.
2. **Active Tasks**: Bulleted list of active technical or operational workstreams.
3. **Why It Matters**: Core architectural, business, reliability, or strategic motivation.
4. **Blockers & Issues**: Specific bottlenecks, dependency limits, or defects (`None` if clear).
5. **Impact of Inaction**: Explicit `Risk Level` (`High`, `Medium`, or `Low`) and quantified consequences if delayed.
6. **Alternative Solutions**: `Option A (Optimal Solution)`, `Option B (Workaround / Fallback)`, and `Recommended Next Step`.

<hr />

## Installation

This repository distributes a standalone skill named `project-status-briefing`. Clone the repository first:

```bash
git clone [https://github.com/KingsleyHK0323/AI_Project_Status_Briefing.git](https://github.com/KingsleyHK0323/AI_Project_Status_Briefing.git)
cd AI_Project_Status_Briefing
```

Install `SKILL.md` into your AI assistant environment:

<details>
<summary><b>Claude Code (CLI)</b></summary>

Copy `SKILL.md` into your global or project-level skills directory:

```bash
# Global installation
mkdir -p ~/.claude/skills/project-status-briefing
cp SKILL.md ~/.claude/skills/project-status-briefing/SKILL.md

# Or project-scoped installation
mkdir -p .claude/skills/project-status-briefing
cp SKILL.md .claude/skills/project-status-briefing/SKILL.md
```

</details>

<details>
<summary><b>Claude (Web & Desktop Apps)</b></summary>

Package the `project-status-briefing` folder containing `SKILL.md` into a `.zip` archive and upload it through **Settings → Capabilities / Skills** (refer to Anthropic's documentation for current UI labels).

</details>

<details>
<summary><b>Cursor, Gemini, ChatGPT, and Custom Agents</b></summary>

For tools that do not load `SKILL.md` natively, paste the Markdown body of `SKILL.md` (everything below the closing `---` frontmatter line) into your assistant's rules file, custom instructions, or system prompt.

</details>

<hr />

## Usage

Paste raw notes or ask for a status report directly:

```text
Turn these notes into a status briefing: API migration is 70% done, auth token
refresh has a 500 bug on staging, release target is Friday.
```

The assistant returns a structured six-section briefing in English with an explicit risk rating, optimal/fallback options, and a recommended immediate next step.

<hr />

## Repository Structure

```text
.
├── SKILL.md      # Standard AI skill specification (frontmatter, rules, six-part structure, checklist)
├── README.md     # Repository overview, output schema, and installation guide
└── LICENSE       # MIT License
```

<hr />

## Contributing

Contributions are welcome, especially improvements to reporting clarity and edge-case handling.

1. Fork the repository and create a branch (`git checkout -b feat/improve-risk-guidance`).
2. Update `SKILL.md` (and `README.md` if documentation changes), keeping YAML frontmatter (`name` and `description`) valid.
3. Verify that all six output sections and risk tags remain consistent.
4. Open a pull request describing the change.

<hr />

## License

Released under the [MIT License](LICENSE). Copyright (c) 2026 Kingsley ([@KingsleyHK0323](https://github.com/KingsleyHK0323)).