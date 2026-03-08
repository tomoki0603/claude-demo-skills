# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

## Repository Overview

Claude Code のカスタムスキル集リポジトリ。スキルファイル（`SKILL.md`）と参照ファイル（`references/`）で構成される。
GitHub: https://github.com/tomoki0603/claude-demo-skills

## Project Structure

```
.claude/skills/          — スキル本体（Claude Code が自動ロード）
.mcp.json                — MCP サーバー設定（Playwright）
nikkei-summaries/        — 日経ブリーフィング出力フォルダ
```

## Available Skills

新しいスキルを追加する際は、このセクションを更新してトリガーワードの重複を防ぐこと。

| スキル名 | 用途 | 主なトリガーワード |
|---------|------|----------------|
| `nikkei-investment-briefing` | 日経電子版の投資ニュースを収集・要約 | 「日経をまとめて」「朝刊をチェックして」「夕刊を追加して」 |
| `skill-creator-max` | 新規スキルを対話形式で設計・生成 | 「新しいスキルを作りたい」「スキルを設計したい」「skill-creator-maxを使って」 |

## Adding New Skills

1. `.claude/skills/<skill-name>/SKILL.md` を作成する
2. 上記テーブルにスキル名・用途・トリガーワードを追記する
3. 既存スキルとトリガーワードが重複しないか確認する
4. 変更を commit して push する

## MCP Configuration

`.mcp.json` に Playwright MCP を設定済み（Windows 環境）。
新しい MCP を追加する場合は `.mcp.json` を編集し、Claude Code を再起動すること。
