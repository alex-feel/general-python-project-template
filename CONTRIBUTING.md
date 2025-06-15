# Contributing

Thank you for your interest in contributing to the project! We appreciate your help in improving our retrieval service, core components, and documentation.

Please follow these guidelines when making contributions.

## Commit Conventions

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification to maintain a clear and consistent commit history.

### Types and Scopes

Below are the conventional commit types we use:

#### feat

For new features or graph implementations:

- No scopes needed.
- Example: `feat: implement some feature`
- Example: `feat: add some functionality`

#### fix

For bug fixes or reverting previous commits:

- No scopes needed.
- Example: `fix: resolve some issue`
- Example: `fix: handle some case`

#### chore

For maintenance tasks and infrastructure:

- No scopes needed.
- Example: `chore: update some dependency to v0.1.0`
- Example: `chore: optimize some process`
- Example: `chore: refactor some code`

#### docs

For documentation improvements:

- No scopes needed.
- Example: `docs: update some documentation`
- Example: `docs: add some diagram`

#### ci

For changes to CI/CD configuration files and pipelines:

- No scopes needed.
- Example: `ci: add some deployment workflow`
- Example: `ci: update some settings`

#### test

For test-related changes (actual test code):

- No scopes needed.
- Example: `test: add some tests`
- Example: `test: cover some cases`

## Pull Request Process

1. **Fork** the repository and create a feature branch from `main`
2. Ensure your changes follow our architecture
3. Update documentation if needed
4. Include relevant tests for new features
5. Submit a Pull Request with a clear description of changes

## Additional Guidelines

- **pre-commit Hooks**: This project uses [pre-commit](https://pre-commit.com/) to ensure code quality and consistency. After cloning the repository, please run `pre-commit install` in the project root to enable automatic formatting, linting, and other checks on every commit.
- Ensure your code follows our style conventions.
- If you add a new feature or fix a bug, please provide tests.
- All features should adhere to the existing architecture and design principles of the project.

Thank you for contributing to the project!
