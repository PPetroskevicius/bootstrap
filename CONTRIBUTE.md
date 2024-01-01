# Contributing

## Commit Message Conventions

This project follows the Conventional Commits standard for structuring commit messages. Commit messages should have the following format:

`<type>(<scope>): <message>`


### Commit Message Components:

- `<type>`: Describes the purpose of the commit. Choose from the following types:
  - `feat`: A new feature or enhancement.
  - `fix`: A bug fix.
  - `docs`: Documentation updates.
  - `chore`: Routine tasks, maintenance, or tooling changes.
  - `style`: Code style changes (e.g., formatting).
  - `refactor`: Code refactoring without new features or fixes.
  - `test`: Adding or modifying tests.
  - `perf`: Performance improvements.
  - `revert`: Reverting a previous commit.

- `<scope>` (Optional): Describes the scope or module of the project that the commit affects.

- `<message>`: A concise description of the change or work done in the commit.

### Examples:

- `feat(user-auth): Add user registration functionality`
- `fix(api-bug): Resolve null pointer issue in API`
- `docs(readme): Update installation instructions`

## Usage Guidelines

### Valid <type> Values:

- `feat`: When adding a new feature or enhancement.
- `fix`: For bug fixes.
- `docs`: When making documentation updates.
- `chore`: For routine tasks, maintenance, or tooling changes.
- `style`: Code style changes like formatting.
- `refactor`: Code refactoring without adding new features or fixing issues.
- `test`: Adding or modifying tests.
- `perf`: Performance improvements.
- `revert`: When reverting a previous commit.

### Using <scope> (Optional):

- Use `<scope>` when it provides additional context about where the changes occurred.
- Examples of <scope> usage: `user-auth`, `api-bug`, `readme`.

## Tools and Integration

- We use tools like Commitizen and Commitlint to enforce commit message conventions.
- Make sure to install and configure these tools in your development environment.

## Changelog Generation

- Commit messages following these conventions are used to automatically generate changelogs for releases.
- This helps maintain a clear history of changes and facilitates version tracking.

## Enforcement and Code Review

- All commits will be reviewed for adherence to these conventions during code reviews.
- Ensure your commits follow the specified format to streamline the review process.

## Questions and Assistance

If you have any questions or need assistance regarding commit message conventions or any other project-related matters, please reach out to [Your Contact Information or Support Channels].


Thank you for contributing to our project and following these guidelines to maintain a clean and informative commit history!
