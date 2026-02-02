# Curator

Curator is a Claude Code configuration focused on Obsidian knowledge management and productivity optimization.

## Project Structure

```
curator/
├── agents/           # Agent configurations (planned)
├── commands/         # Command templates (planned)
├── hooks/            # Hook scripts (planned)
├── skills/           # Specialized skills
└── settings          # Configuration files
```

## Commands

| Command       | Status | Description               |
| ------------- | ------ | ------------------------- |
| brainstorm    | WIP    | Brainstorming template    |
| init-vault    | WIP    | Initialize Obsidian vault |
| kick-off      | WIP    | Project kickoff template  |
| start-new-day | WIP    | Daily planning template   |

## Skills

| Skill                                                              | Status | Description                                                                         |
| ------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------- |
| [beautiful-mermaid-diagrams](./skills/beautiful-mermaid-diagrams/) | Ready  | Create beautiful Mermaid diagrams (flowcharts, sequence, class, ER, state diagrams) |
| [obsidian-moc-creator](./skills/obsidian-moc-creator/)             | Ready  | Create structured MOC (Map of Content) documents for knowledge organization         |

## Planned Features

- Agent configurations for automated workflows
- Hook scripts for event-driven automation
- Session templates for recurring tasks

## Usage

```shell
skills add blackcater/curator -g
```
