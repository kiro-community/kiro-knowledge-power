# GitHub Issues Search Workflow

Search [GitHub Issues](https://github.com/kirodotdev/Kiro/issues) when official documentation and community knowledge base cannot resolve the issue.

## Search Steps

### Step 1: Prepare Search Keywords

Translate Chinese questions to English keywords:

**Examples**:

- "如何配置 MCP" → "how to configure MCP"
- "插件安装失败" → "plugin installation failed"
- "性能问题" → "performance issue"

### Step 2: Use GitHub MCP Search

Use **github** MCP's search_issues tool:

```
Parameters:
  - repo: kirodotdev/Kiro
  - query: [English keywords]
  - state: all (search all states)
```

### Step 3: Analyze Search Results

**Priority Sorting**:

1. Closed Issues with solution (resolved issues)
2. Open Issues with workaround (with temporary solutions)
3. Recent discussions (recent discussions)

**Extract Information**:

- Problem description
- Solution
- Related discussions
- Official responses
