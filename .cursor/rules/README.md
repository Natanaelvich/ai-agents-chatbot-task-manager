# Cursor Rules Documentation

This project uses Cursor Rules to maintain consistent code quality and development patterns.

## 📁 Rule Files

### 1. `project.mdc` - Project Guidelines
- **Scope**: Global project rules
- **Applies to**: All files
- **Purpose**: Core project architecture, routing, and general guidelines

### 2. `react-components.mdc` - React Components
- **Scope**: React components
- **Applies to**: `**/*.tsx`, `**/*.jsx`
- **Purpose**: Component structure, props, state management, styling

### 3. `typescript.mdc` - TypeScript Guidelines
- **Scope**: TypeScript files
- **Applies to**: `**/*.ts`, `**/*.tsx`
- **Purpose**: Type definitions, imports/exports, type safety

### 4. `ai-features.mdc` - AI Features
- **Scope**: AI and chatbot features
- **Applies to**: Chat interface and AI-related files
- **Purpose**: Message handling, AI integration patterns

### 5. `commit-guidelines.mdc` - Commit Guidelines
- **Scope**: Git commits and version control
- **Applies to**: All files (always apply)
- **Purpose**: Commit structure, grouping rules, message formatting

## 🎯 How to Use

1. **Automatic Application**: Rules are automatically applied when editing files
2. **File-Specific**: Rules apply based on file patterns (globs)
3. **Always Apply**: Some rules apply to all files regardless of type
4. **Contextual**: Rules provide relevant suggestions based on file content

## 📝 Adding New Rules

To add a new rule:

1. Create a new `.mdc` file in `.cursor/rules/`
2. Use the following structure:
```markdown
---
description: Rule description
globs: ["file-patterns"]
alwaysApply: true/false
---

# Rule Title

## Guidelines
- Rule 1
- Rule 2

## Examples
```typescript
// Code examples
```
```

## 🔧 Rule Priorities

1. **Project Rules** (highest priority)
2. **Commit Guidelines** (high priority - always apply)
3. **File-Specific Rules** (medium priority)
4. **Feature-Specific Rules** (contextual priority)

## 📚 Best Practices

- Keep rules concise and actionable
- Include code examples
- Use clear, descriptive language
- Update rules as project evolves
- Test rules with actual development scenarios 