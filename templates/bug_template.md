# 🐞 Debugging Assistant Configuration

## 🎯 Purpose
Guide the AI agent to effectively debug and fix issues in the codebase by providing structured context and clear instructions.

## 📋 Project Context
```
Project Path: [Full path to project root]
Project Type: [e.g., React/Node.js/TypeScript/Python]
Main Entry Point: [e.g., src/index.ts, app/main.py]
```

## 🧩 Current Issue
```
[Provide detailed description of the bug or issue]

Error Message (if any):
[Paste error message here]

Affected Components:
- [Component/File 1]
- [Component/File 2]
```

## 🛠️ Debugging Instructions

### 1. Codebase Exploration
- Map the codebase structure starting from the main entry point
- Identify key components and their relationships
- Document the execution flow related to the issue

### 2. Issue Analysis
- Reproduce the issue in a controlled environment
- Add debug logs at critical points
- Identify the root cause by tracing through the execution flow

### 3. Solution Implementation
- Propose a fix with minimal changes
- Ensure backward compatibility
- Add/update tests to prevent regression

## 📝 Output Format
```markdown
## Investigation Notes
[Agent's detailed analysis]

## Proposed Solution
[Detailed explanation of the fix]

## Changes Made
```diff
[Git-style diff of changes]
```

## Testing Instructions
1. [Step 1 to test]
2. [Step 2 to verify]

## 🔄 Workflow Preferences
- Use `bun test` for running tests
- Create feature branches for fixes: `fix/description-of-fix`
- Follow existing code style and patterns
- Document any new patterns or architectural decisions

## 🚀 Getting Unstuck
If stuck after [X] attempts:
1. Summarize findings
2. List attempted solutions
3. Identify specific areas needing clarification
4. Request human assistance with specific questions

## 📚 Additional Resources
- [Link to project documentation]
- [Link to relevant API docs]
- [Link to style guide]