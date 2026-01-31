# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Lenny's Wisdom is a Claude Code plugin that surfaces expert frameworks from Lenny's Podcast guests. It provides decision support and implementation guidance through diagnostic questions that match users with relevant experts.

## Architecture

This is a Claude Code plugin with the following structure:

- **`.claude-plugin/plugin.json`** - Plugin manifest defining metadata
- **`skills/<skill-name>/SKILL.md`** - Auto-discovered skills containing expert frameworks, each with:
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

1. Create a new directory in `skills/` named after the skill (e.g., `skills/lennys-newskill/`)
2. Create `SKILL.md` inside that directory
3. Add YAML frontmatter with `name` and `description`
4. Follow the diagnostic → frameworks → delivery pattern from existing skills

Skills are auto-discovered — no need to register in plugin.json.

## Skills

| Skill | Directory |
|-------|-----------|
| `/lennys-growth` | skills/lennys-growth/SKILL.md |
| `/lennys-product-strategy` | skills/lennys-product-strategy/SKILL.md |
| `/lennys-sales` | skills/lennys-sales/SKILL.md |
| `/lennys-story` | skills/lennys-story/SKILL.md |
| `/lennys-leadership` | skills/lennys-leadership/SKILL.md |
| `/lennys-career` | skills/lennys-career/SKILL.md |
| `/lennys-ai` | skills/lennys-ai/SKILL.md |
| `/lennys-behavior` | skills/lennys-behavior/SKILL.md |
| `/lennys-founder` | skills/lennys-founder/SKILL.md |
| `/lennys-marketplace` | skills/lennys-marketplace/SKILL.md |
