# Quality Check

## Contents
- [Quality Check](#quality-check)
  - [Contents](#contents)
  - [Pre-generation Check](#pre-generation-check)
  - [Depth Validation](#depth-validation)
  - [Content Check](#content-check)
    - [Relevance](#relevance)
    - [Structure](#structure)
    - [Depth](#depth)
  - [Format Check](#format-check)
    - [Wikilinks](#wikilinks)
    - [Frontmatter](#frontmatter)
    - [Code Blocks](#code-blocks)
  - [Completeness Check](#completeness-check)
  - [Validation Checklist](#validation-checklist)
  - [Quality Scores](#quality-scores)

---

## Pre-generation Check

Before generating MOC, verify:

- [ ] **Intent clear**: User's goal is understood
- [ ] **Depth level confirmed**: beginner / intermediate / advanced / interview
- [ ] **Topic scope defined**: Boundaries of the MOC
- [ ] **Existing notes checked**: Links to existing Obsidian notes

---

## Depth Validation

| Depth            | Expected Sections                                         |
| ---------------- | --------------------------------------------------------- |
| **beginner**     | Overview, Core Concepts, Getting Started, Basic Resources |
| **intermediate** | All standard modules                                      |
| **advanced**     | All standard + Best Practices, Source Analysis            |
| **interview**    | All standard + Interview Q&A, Strategy                    |

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
- [ ] Interview mode: Covers common interview questions

---

## Format Check

Check Obsidian formatting:

### Wikilinks
- [ ] Use `[[page name]]` for internal links
- [ ] No broken links
- [ ] Links point to likely existing pages

### Frontmatter
```yaml
---
title: [Title]
tags:
  - moc
  - [topic]
type: moc
created: [YYYY-MM-DD]
updated: [YYYY-MM-DD]
---
```

### Code Blocks
- [ ] Language specified: `\`\`\`python`
- [ ] Code is correct and idiomatic
- [ ] Comments explain non-obvious parts

---

## Completeness Check

- [ ] No placeholder text like "TODO" or "内容待补充"
- [ ] All wikilinks have meaningful targets
- [ ] External links are valid URLs
- [ ] No section is overly thin or excessively detailed
- [ ] Consistent terminology throughout

---

## Validation Checklist

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
