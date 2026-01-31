---
name: create-moc
description: Create structured MOC (Map of Content) documents for programmers. Use when users want to organize knowledge, prepare for interviews, or learn new technologies. Triggers: "MOC", "内容地图", "知识整理", "面试准备", "学习路线".
---

# Obsidian MOC Creator

Create comprehensive, well-structured MOC documents for learning, interview preparation, and project documentation.

## Quick Start

1. **Identify scenario**: learning / interview / project
2. **Determine depth**: beginner / intermediate / advanced
3. **Generate MOC**: Use appropriate template

## Scenarios

Choose the right approach based on user's intent:

| Scenario      | Description                         | Keywords                   |
| ------------- | ----------------------------------- | -------------------------- |
| **Learning**  | Systematic knowledge acquisition    | 学习, 入门, 教程, 掌握     |
| **Interview** | Technical interview preparation     | 面试, 面经, 刷题, P6/P7    |
| **Project**   | Project documentation and reference | 项目, 技术方案, 架构, 文档 |

**Details**: See [SCENARIOS.md](reference/scenarios.md)

## Templates

Use the appropriate template for the scenario:

### Learning Template
For systematic learning of new technologies.
**Template**: Use [TEMPLATES.md](reference/templates/template-learning.md)

### Interview Template
For technical interview preparation.
**Template**: Use [TEMPLATES.md](reference/templates/template-interview.md)

### Project Template
For project documentation and knowledge sharing.
**Template**: Use [TEMPLATES.md](reference/templates/template-project.md)

### Mini Template
For quick reference on simple topics.
**Template**: Use [TEMPLATES.md](reference/templates/template-mini.md)

## Workflow

Copy and track progress:

```
MOC Creation:
- [ ] Step 1: Analyze request and identify scenario
- [ ] Step 2: Determine depth level with user
- [ ] Step 3: Create a directory (`10_MOC/[topic]` or `10_MOC/[topic]-[scenario]`) to store all generated files
- [ ] Step 4: Select appropriate template
- [ ] Step 5: Generate MOC structure
- [ ] Step 6: Fill content based on knowledge
- [ ] Step 7: Apply output format
- [ ] Step 8: Validate quality
```

**Detailed workflow**: Follow the quality checklist in [QUALITY_CHECK.md](reference/quality-check.md)

## Output Format

All MOC files must follow Obsidian conventions:

- Filename: kebab-case
- YAML frontmatter for properties
- Proper wikilinks `[[page name]]`
- Correct code block syntax
- Appropriate callouts

**Specification**: See [OUTPUT_FORMAT.md](reference/output-format.md)

## Quality Standards

Before finalizing, validate:

- [ ] All sections have meaningful content
- [ ] Wikilinks are correctly formatted
- [ ] No placeholder text
- [ ] Consistent terminology
- [ ] Proper heading hierarchy

**Checklist**: See [QUALITY_CHECK.md](reference/quality-check.md)

## Tips

- **Keep it actionable**: Each node should point to real content
- **Link early**: Add `[[ ]]` links even if pages don't exist yet
- **Iterate**: MOCs evolve as knowledge grows
- **Balance**: Avoid both too sparse and too detailed
