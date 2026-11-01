# Architecture

## English

### Purpose

The architecture separates canonical knowledge, raw inputs, operational state, and compact exports. This makes changes traceable and prevents an AI assistant's memory from becoming an uncontrolled copy of the vault.

### Components

- **Canonical vault:** local Markdown files containing curated knowledge.
- **Inbox:** unprocessed conversations, documents, and other sources.
- **Operational memory:** current state, decisions, open loops, and preferences.
- **Curated layer:** notes, areas, topics, projects, people, and maps of content.
- **Exports:** compact web handoffs and memory digests derived from canonical files.
- **Metadata:** indexes, content hashes, reports, and patches.

### Data flow

1. A source enters the inbox or is converted into a session pack.
2. An assistant extracts state-changing information.
3. A dry-run describes proposed changes without applying them.
4. The user confirms or corrects the proposal.
5. Canonical files and indexes are updated.
6. Reports, patches, handoffs, and digests are regenerated.

### Source priority

1. Explicit current user instructions.
2. Current STATE, decisions, and open loops.
3. Curated notes and maps of content.
4. Raw inbox sources as untrusted context.

### Traceability

Each canonical document should have a stable path and a content hash. Derived exports should identify their canonical sources so that stale mirrors can be detected.

## Русский

### Назначение

Архитектура разделяет канонические знания, сырые входы, оперативное состояние и компактные экспорты. Это обеспечивает трассируемость изменений и не позволяет памяти ИИ-ассистента превратиться в неконтролируемую копию vault.

### Компоненты

- **Canonical vault:** локальные Markdown-файлы с курируемыми знаниями.
- **Inbox:** необработанные диалоги, документы и другие источники.
- **Оперативная память:** текущее состояние, решения, открытые вопросы и предпочтения.
- **Курируемый слой:** заметки, области, темы, проекты, люди и карты знаний.
- **Экспорты:** компактные web handoffs и memory digests, производные от canonical-файлов.
- **Метаданные:** индексы, content hashes, отчёты и patches.

### Поток данных

1. Источник попадает в inbox или преобразуется в session pack.
2. Ассистент извлекает информацию, изменяющую состояние базы.
3. Dry-run описывает предлагаемые изменения без их применения.
4. Пользователь подтверждает или корректирует предложение.
5. Обновляются canonical-файлы и индексы.
6. Пересоздаются отчёты, patches, handoffs и digests.

### Приоритет источников

1. Явные текущие инструкции пользователя.
2. Актуальные STATE, decisions и open loops.
3. Курируемые заметки и карты знаний.
4. Сырые источники из inbox как недоверенный контекст.

### Трассируемость

Каждый canonical-документ должен иметь стабильный путь и content hash. Производные экспорты должны указывать свои canonical-источники, чтобы можно было обнаружить устаревшие зеркала.
