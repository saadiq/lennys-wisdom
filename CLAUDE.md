# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Lenny's Wisdom is a Claude Code plugin that surfaces expert frameworks from Lenny's Podcast guests. It provides decision support and implementation guidance through diagnostic questions that match users with relevant experts.

## Architecture

This is a Claude Code plugin with the following structure:

- **`.claude-plugin/plugin.json`** - Plugin manifest defining metadata and skill registrations
- **`skills/`** - Markdown files containing expert frameworks, each with:
  - YAML frontmatter (`name`, `description`) for skill metadata
  - Diagnostic questions to understand user context
  - Expert frameworks with attribution, core insights, and implementation steps
  - Delivery guidelines for presenting frameworks

## Skill Pattern

Each skill follows a consistent structure:
1. **Diagnostic Process** - Sequential questions asked one at a time
2. **Expert Frameworks** - Each expert has background info and multiple frameworks containing:
   - Core insight (key principle in 1-2 sentences)
   - The problem it solves
   - Implementation steps
   - When to apply
3. **Delivery Guidelines** - How to present frameworks to users

## Adding New Skills

1. Create a new markdown file in `skills/`
2. Add YAML frontmatter with `name` and `description`
3. Register in `.claude-plugin/plugin.json` under the `skills` array
4. Follow the diagnostic → frameworks → delivery pattern from existing skills

## Skill Commands

| Command | Skill File |
|---------|------------|
| `/growth` | skills/growth-activation.md |
| `/product-strategy` | skills/product-strategy.md |
| `/sales` | skills/sales-gtm.md |
| `/story` | skills/storytelling.md |
| `/leadership` | skills/leadership.md |
| `/career` | skills/career.md |
| `/ai` | skills/ai-future.md |
| `/behavior` | skills/behavioral-design.md |
| `/founder` | skills/founder-essentials.md |
| `/marketplace` | skills/marketplaces.md |
