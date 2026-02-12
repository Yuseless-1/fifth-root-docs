# Contributing to Fifth Root Documentation

Thank you for your interest in contributing to Fifth Root's documentation!

## How to Contribute

### Reporting Issues

Found an error or outdated information?

1. Check if the issue already exists
2. Open a GitHub issue with:
   - Clear title
   - Description of the problem
   - Suggested fix (if applicable)
   - Link to affected section

### Submitting Changes

To submit documentation changes:

1. **Fork** the repository
2. **Create a branch** for your changes
   ```bash
   git checkout -b fix/description-of-fix
   ```
3. **Make your changes** following the guidelines below
4. **Commit** with clear messages
   ```bash
   git commit -m "Fix: correct spelling in character evolution section"
   ```
5. **Push** to your fork
6. **Create a Pull Request** with description

## Documentation Style Guide

### Structure

- Use clear headings hierarchy (H1 → H2 → H3)
- Keep sections focused and concise
- Use tables for data comparisons
- Include code blocks for technical content

### Writing Style

- Use second person ("you can plant seeds")
- Active voice preferred
- Technical but accessible
- Consistent terminology
- Real examples where helpful

### Formatting

- **Bold** for UI elements and important terms
- *Italics* for emphasis
- `Code blocks` for game terms and mechanics
- Lists for step-by-step processes
- Tables for stat comparisons

### Game Terminology

Maintain consistent terminology:
- "Aether" (not "aether" or "AETHER")
- "Root" / "Roothi" (proper nouns)
- "Guild" vs "guild" (capitalize when referring to the system)
- "Sprite" (capitalized when referring to game object)
- "XP" (not "exp" or "experience")

## Content Guidelines

### Game Systems
- Document complete mechanics
- Include stat tables where relevant
- Explain progression requirements clearly
- Provide examples of gameplay flow

### Technical Content
- Explain architecture clearly
- Use diagrams for complex systems
- Include database schema details
- Reference API endpoints precisely

### Balance Information
- Include stat values and progressions
- Explain evolution requirements
- Detail reward systems
- Clarify cooldowns and resource costs

## File Organization

```
docs/
├── 01-build-guide.md          # Development guide
├── 02-game-architecture.md    # Technical backend
├── 03-character-creation.md   # Onboarding
├── 04-level-1-gameplay.md     # Core gameplay
├── 05-character-evolution.md  # Progression
├── 06-sprites-abilities.md    # Combat system
└── 07-events-system.md        # Tournaments & Raids
```

Add new docs in numerical order with descriptive names.

## Review Process

1. PRs are reviewed for:
   - Accuracy of game mechanics
   - Consistency with existing docs
   - Clarity and readability
   - Formatting compliance
2. Changes may be requested before merge
3. Once approved, changes are merged and deployed

## Questions?

- Open a GitHub discussion
- Tag @Reviewer for urgent issues
- Check existing docs first for answers

---

**Thanks for helping make Fifth Root documentation better!**
