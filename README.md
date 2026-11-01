# Assistant-Maintained Second Brain

## English

A reusable set of protocols and templates for building a Second Brain where a local Markdown vault is the canonical source of truth and AI assistants help capture, process, and maintain knowledge under user supervision.

**Version:** v0.3  
**Status:** Active template project

### Core principles

- The local vault is the canonical source of truth.
- AI memory is only a compact digest, not a copy of the vault.
- Users provide sources and approvals; assistants maintain the structure.
- Canonical changes are reviewed before being applied.
- Unknown facts are never invented; hypotheses are explicitly labelled.
- Secrets, private records, and sensitive personal data must not enter the public repository.
- Raw sources remain separate from curated knowledge.

### Repository contents

- Architecture and workflow documentation.
- Session pack template.
- STATE, decisions, and open-loops templates.
- Web handoff and memory digest templates.
- Example index structure.
- Privacy and safety guidelines.

### Basic workflow

1. Capture a conversation or source as a session pack.
2. Run a dry-run ingest.
3. Review proposed creations, updates, duplicates, and conflicts.
4. Confirm or correct the proposed changes.
5. Update the canonical vault.
6. Record a report and patch.
7. Refresh the compact handoff and memory digest.

### Suggested vault structure

- `10_inbox/` — raw inputs and session packs.
- `20_memory/` — STATE, decisions, open-loops, and operational notes.
- `30_notes/`, `40_areas/`, `50_topics/`, `60_projects/`, `70_people/` — curated knowledge.
- `80_moc/` — maps of content.
- `95_exports/` — compact handoffs and memory digests.
- `99_meta/` — protocols, templates, indexes, reports, and patches.

### Privacy boundary

This repository contains generic documentation and empty templates only. It must not contain real personal notes, private exports, account data, credentials, API keys, tokens, or sensitive records.

## Русский

Набор универсальных протоколов и шаблонов для создания Second Brain, в котором локальный Markdown-vault является каноническим источником истины, а ИИ-ассистенты помогают собирать, обрабатывать и поддерживать знания под контролем пользователя.

**Версия:** v0.3  
**Статус:** Активный шаблонный проект

### Основные принципы

- Локальный vault — канонический источник истины.
- Память ИИ — только компактный дайджест, а не копия vault.
- Пользователь предоставляет источники и подтверждения; ассистенты поддерживают структуру базы.
- Изменения canonical-слоя проверяются до применения.
- Неизвестные факты не выдумываются; гипотезы явно помечаются.
- Секреты, приватные записи и чувствительные персональные данные не должны попадать в публичный репозиторий.
- Сырые источники хранятся отдельно от курируемых знаний.

### Содержимое репозитория

- Документация по архитектуре и рабочим процессам.
- Шаблон session pack.
- Шаблоны STATE, decisions и open-loops.
- Шаблоны web handoff и memory digest.
- Пример структуры индекса.
- Рекомендации по приватности и безопасности.

### Базовый рабочий процесс

1. Сохранить диалог или источник как session pack.
2. Выполнить dry-run ingest.
3. Проверить предлагаемые создания, обновления, дубли и конфликты.
4. Подтвердить или скорректировать изменения.
5. Обновить canonical-vault.
6. Зафиксировать отчёт и patch.
7. Обновить компактный handoff и memory digest.

### Рекомендуемая структура vault

- `10_inbox/` — сырые входы и session packs.
- `20_memory/` — STATE, decisions, open-loops и оперативные заметки.
- `30_notes/`, `40_areas/`, `50_topics/`, `60_projects/`, `70_people/` — курируемые знания.
- `80_moc/` — карты знаний.
- `95_exports/` — компактные handoffs и memory digests.
- `99_meta/` — протоколы, шаблоны, индексы, отчёты и patches.

### Граница приватности

Репозиторий содержит только общую документацию и пустые шаблоны. В нём не должно быть реальных личных заметок, приватных выгрузок, данных аккаунтов, учётных данных, API-ключей, токенов или чувствительных записей.
