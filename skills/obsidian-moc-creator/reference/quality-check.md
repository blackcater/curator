# Quality Check

## Contents
- [Quality Check](#quality-check)
  - [Contents](#contents)
  - [Pre-generation Check](#pre-generation-check)
  - [Content Check](#content-check)
    - [Relevance](#relevance)
    - [Structure](#structure)
    - [Depth](#depth)
  - [Format Check](#format-check)
    - [Wikilinks](#wikilinks)
    - [Callouts](#callouts)
    - [Lists](#lists)
    - [Code Blocks](#code-blocks)
  - [Completeness Check](#completeness-check)
    - [Required Sections](#required-sections)
    - [Missing Items](#missing-items)
    - [Balance](#balance)
  - [Validation Checklist](#validation-checklist)
  - [Quick Validation Commands](#quick-validation-commands)
  - [Quality Scores](#quality-scores)

---

## Pre-generation Check

Before generating MOC, verify:

- [ ] **Intent clear**: User's goal is understood
- [ ] **Scenario identified**: learning / interview / project
- [ ] **Depth level confirmed**: beginner / intermediate / advanced
- [ ] **Topic scope defined**: Boundaries of the MOC
- [ ] **Existing notes checked**: Links to existing Obsidian notes

---

## Content Check

Verify MOC content quality:

### Relevance
- [ ] All sections relate to the topic
- [ ] No irrelevant or generic content
- [ ] Depth matches user's level

### Structure
- [ ] Hierarchical headings are logical
- [ ] Sections flow in learning order
- [ ] Cross-references exist where needed

### Depth
- [ ] Key concepts are explained, not just listed
- [ ] Examples provided for important concepts
- [ ] Links to deeper resources for advanced users

---

## Format Check

Check Obsidian formatting:

### Wikilinks
- [ ] Use `[[page name]]` for internal links
- [ ] No broken links
- [ ] Links point to likely existing pages

### Callouts
- [ ] Use `> [!info]` for notes
- [ ] Use `> [!warning]` for cautions
- [ ] Use `> [!tip]` for tips

### Lists
- [ ] Consistent bullet style
- [ ] Proper indentation
- [ ] Meaningful list items

### Code Blocks
- [ ] Language specified: `\`\`\`python`
- [ ] Code is correct and idiomatic
- [ ] Comments explain non-obvious parts

---

## Completeness Check

Ensure MOC is comprehensive:

### Required Sections
| Scenario  | Required Sections                            |
| --------- | -------------------------------------------- |
| Learning  | Overview, Core Concepts, Practice, Resources |
| Interview | Basics, Advanced, Projects, Coding           |
| Project   | Overview, Architecture, Pitfalls, Ops        |

### Missing Items
- [ ] No placeholder text like "TODO"
- [ ] No "内容待补充" or similar
- [ ] All links have targets

### Balance
- [ ] No section is overly thin
- [ ] No section is excessively detailed
- [ ] Proportions make sense for the topic

---

## Validation Checklist

Copy and complete this checklist before finalizing:

```
MOC Quality Validation:
- [ ] Topic is clearly defined at top
- [ ] Purpose of MOC is stated
- [ ] Target audience is implied or stated
- [ ] All main sections have content
- [ ] Sub-sections have meaningful details
- [ ] Links point to existing or likely notes
- [ ] External links are valid URLs
- [ ] Code examples are correct
- [ ] No grammatical errors
- [ ] Consistent terminology
- [ ] Obsidian syntax is correct
- [ ] File name matches topic (kebab-case)
```

---

## Quick Validation Commands

```bash
# Check for common issues
grep -n "TODO\|待补充\|TODO" obsidian-moc.md

# Verify wikilinks (basic)
grep -o '\[\[.*\]\]' obsidian-moc.md | wc -l

# Count sections
grep -n "^## " obsidian-moc.md | wc -l
```

---

## Quality Scores

Rate the MOC on these dimensions (1-5):

| Dimension    | Score | Notes |
| ------------ | ----- | ----- |
| Completeness | /5    |       |
| Structure    | /5    |       |
| Clarity      | /5    |       |
| Usefulness   | /5    |       |
| Links        | /5    |       |

**Target**: Average score of 4.0 or higher
