# Contributing to Meduseld Site

## Commit Message Format

We use [Conventional Commits](https://www.conventionalcommits.org/) for all commit messages. This is enforced automatically via git hooks.

### Format

```
<type>(<scope>): <subject>

[optional body]

[optional footer]
```

### Types

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

### Scopes

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

### Examples

```bash
feat(services): integrate Steam news feed
fix(system): resolve log loading error
style(footer): update copyright year
refactor(ui): consolidate button styles
docs(readme): add setup instructions
```

### Using Commitizen (Recommended)

For an interactive commit prompt:

```bash
npm run commit
```

This will guide you through creating a properly formatted commit message.

### Setup for Contributors

1. Clone the repository
2. Run `npm install` to install dependencies
3. Husky will automatically set up git hooks
4. Use `npm run commit` or commit normally (validation will run automatically)

### Breaking Changes

For breaking changes, add `!` after the type:

```bash
feat(ui)!: redesign service cards layout
```

### Pull Requests

- Keep PRs focused on a single feature or fix
- Write clear PR descriptions
- Reference related issues
- Ensure all commits follow the format
- Update CHANGELOG.md if needed
