# Project Pulse Agent Team

This document outlines the specialist AI agent team configured in `.github/agents` to plan, design, implement, and validate Mona's **Project Pulse** dashboard.

## Specialist Agent Team Overview

The custom agents defined in `.github/agents/` are organized to provide clear separation of concerns, specialized tool capabilities, and coordinated orchestration:

| Agent Role | Agent Definition File | Assigned Model | Core Responsibility |
|---|---|---|---|
| **Orchestrator** | `.github/agents/orchestrator.agent.md` | Claude Opus 5.5 (copilot) | Coordinates the overall workflow, breaks requests into phases, and delegates tasks to specialists. |
| **Planner** | `.github/agents/planner.agent.md` | Claude Opus 5.5 (copilot) | Develops structured execution plans, file assignments, dependencies, and validation strategy. |
| **Coder** | `.github/agents/coder.agent.md` | GPT-5.5 (copilot) | Implements clean, maintainable frontend code, data fixtures, and launch configurations. |
| **Designer** | `.github/agents/designer.agent.md` | Gemini 3.7 Flash (copilot) | Defines UI/UX hierarchy, responsive layout, accessible styling, and component visual aesthetics. |

## Collaboration Workflow for Project Pulse

1. **Orchestrator** receives the high-level project vision for the Project Pulse dashboard.
2. **Planner** reviews requirements and outputs a concrete implementation roadmap with phase sequencing and dependency mapping.
3. **Designer** establishes the visual identity, responsive grid layout, status badge semantics, and card design.
4. **Coder** implements `app/index.html`, `app/styles.css`, and `app/project-data.json`, alongside `.vscode/launch.json` for preview testing.
5. **Orchestrator** coordinates validation, ensures all files hang together seamlessly, and performs final handoff.
