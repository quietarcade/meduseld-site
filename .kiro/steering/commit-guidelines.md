---
inclusion: auto
---

# Commit Message Guidelines

## CRITICAL: All commits MUST follow Conventional Commits format

When making changes to this repository, you MUST use the following commit format:

```
<type>(<scope>): <subject>

[optional body]

[optional footer]
```

## Types

- `feat`: New feature
- `fix`: Bug fix
- `perf`: Performance improvement
- `refactor`: Code refactoring
- `style`: UI/styling changes
- `docs`: Documentation only
- `test`: Adding/updating tests
- `chore`: Maintenance tasks
- `build`: Build system changes
- `ci`: CI/CD changes

## Scopes for meduseld-site (Frontend)

- `services` - Services hub page
- `system` - System monitor page
- `landing` - Landing page
- `ui` - General UI components
- `icons` - Icon library
- `footer` - Footer component
- `header` - Header component
- `news` - Game news panel
- `prices` - Game pricing
- `release` - Version releases

## Examples

```bash
feat(services): integrate Steam news feed
fix(system): resolve log loading error
style(footer): update copyright year
refactor(ui): consolidate button styles
perf(prices): implement price caching
docs(readme): add setup instructions
chore(deps): update Bootstrap to 5.3.3
```

## Rules

1. **Subject line**: Max 100 characters, sentence case, no period at end
2. **Scope**: Always include a scope (required by commitlint)
3. **Body**: Optional, use for detailed explanations
4. **Footer**: Optional, use for breaking changes or issue references

## Breaking Changes

Add `!` after the type for breaking changes:

```bash
feat(ui)!: redesign service cards layout

BREAKING CHANGE: Old CSS classes removed, update custom styles
```

## Multi-line Commits

```bash
git commit -m "fix(system): improve error handling for log viewer

- Add better error messages for permission issues
- Show helpful hints when logs are unavailable
- Improve loading states

Fixes #15"
```

## Validation

Commits are automatically validated via git hooks. Invalid commits will be rejected with an error message.

## When Making Changes

Always commit your changes using this format. The repository has commitlint configured to enforce these rules.
