# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a Japanese-language documentation repository containing educational guides about Claude Code. There is no build system, source code, or test suite — the content is purely Markdown documentation.

## Contents

- **claude-code-intro.md** — Beginner-friendly introduction to Claude Code: what it is, core capabilities, and how it differs from browser-based AI chat. Written in Japanese.
- **claude-code-skills-guide.md** — Comprehensive technical reference (32KB) covering Skills, slash commands, MCP (Model Context Protocol) server integration, Hooks automation, `.claude` folder structure, and IDE integration. Written in Japanese.

## Document Structure

The skills guide covers these major topics in order:
1. Skills — custom instruction files at `.claude/skills/<name>/SKILL.md`
2. Slash commands — built-in (`/clear`, `/compact`, `/model`, etc.) and skill-based
3. MCP — external tool integration (GitHub, Notion, PostgreSQL, Slack, Stripe) via `.mcp.json`
4. Hooks — event-driven automation (`PreToolUse`, `PostToolUse`, `SessionStart`, `Notification`, `Stop`)
5. `.claude` folder layout — `settings.json`, `settings.local.json`, `CLAUDE.md`, `skills/`, `hooks/`
6. IDE integration — VS Code and JetBrains extensions
7. Practical examples — team coding standards, GitHub issue automation, natural language DB queries
