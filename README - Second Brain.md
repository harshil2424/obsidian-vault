# Second Brain System (PARA)

## Role & Purpose
This vault acts as an autonomous Second Brain Manager. It processes standardized "Handoff Reports" and organizes data according to strict PARA guidelines.

## Vault Architecture

- **`00-Inbox/`**: Unprocessed notes, raw web clips, and external AI handoff files.
- **`01-Projects/`**: Active projects. Each project has an `index.md` tracking goals/tasks.
- **`02-Areas/`**: Broad ongoing technical domains (e.g., Python, JavaScript).
- **`03-Resources/`**: Permanent reference materials, clean code snippets, tools, docs.
- **`04-Archive/`**: Completed projects and deprecated workflows.
- **`05-Templates/`**: Markdown structural templates.
- **`log.md`**: Root-level execution log for actions taken by the autonomous agent.

## Handoff Report Ingestion SOP
When a file matching the structure of a "HANDOFF REPORT" is placed in `00-Inbox/`, the agent will:
1. Identify scope via `METADATA`.
2. Process active projects (update `index.md` and task lists).
3. Extract resources and snippets into `03-Resources/`.
4. Apply links `[[wikilinks]]` and YAML Properties.
5. Log the action in `log.md`.

## Extra Syntax & Formatting
- **Wikilinks**: Used aggressively.
- **Callouts**: `> [!info]`, `> [!warning]`, `> [!todo]`.
- **Math**: `$inline$` or `$$display$$`.
- **Tasks**: strictly `- [ ]` syntax.
