```markdown
# awesome-claude-code Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and conventions used in the `awesome-claude-code` repository, a TypeScript codebase with a focus on clean file organization, consistent import/export styles, and structured testing. Whether you're contributing new features or reviewing code, following these patterns will help maintain code quality and consistency.

## Coding Conventions

### File Naming
- Use **kebab-case** for all file names.
  - Example:  
    ```
    my-component.ts
    utils/helper-functions.ts
    ```

### Import Style
- Use **relative imports** for referencing modules within the project.
  - Example:
    ```typescript
    import { helperFunction } from './utils/helper-functions';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    // In utils/helper-functions.ts
    export function helperFunction() { /* ... */ }
    ```

### Commit Messages
- Commit messages are generally freeform.
- Some commits may use the `[ImgBot]` prefix for automated image updates.
- Keep commit messages concise (average 24 characters).

## Workflows

### Adding a New Feature
**Trigger:** When implementing a new functionality.
**Command:** `/add-feature`

1. Create a new file using kebab-case naming.
2. Implement your feature using TypeScript.
3. Use relative imports to include any dependencies.
4. Export your functions or components using named exports.
5. Write corresponding tests in a `.test.ts` file.
6. Commit your changes with a clear, concise message.

### Refactoring Code
**Trigger:** When improving or restructuring existing code.
**Command:** `/refactor`

1. Identify the code to refactor.
2. Update file names to kebab-case if necessary.
3. Ensure all imports remain relative.
4. Maintain named exports throughout.
5. Run all tests to confirm nothing is broken.
6. Commit with a descriptive message.

### Writing Tests
**Trigger:** When adding or updating tests.
**Command:** `/write-test`

1. Create or update a test file matching the `*.test.*` pattern (e.g., `my-component.test.ts`).
2. Write tests for your functions or components.
3. Use the project's preferred (unknown) testing framework.
4. Run tests to verify correctness.
5. Commit your test changes.

## Testing Patterns

- Test files should follow the `*.test.*` naming convention.
  - Example: `utils.test.ts`
- The specific testing framework is not defined; follow existing patterns in the repository.
- Place tests alongside or near the code they test for clarity.

## Commands
| Command        | Purpose                                      |
|----------------|----------------------------------------------|
| /add-feature   | Start the workflow for adding a new feature  |
| /refactor      | Begin a code refactoring workflow            |
| /write-test    | Guide for writing or updating tests          |
```
