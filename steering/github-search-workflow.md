# GitHub Issues Search Workflow

Search GitHub Issues when official documentation and community knowledge base cannot resolve the issue.

## Search Strategy

### Repository Information
- **Repository**: kirodotdev/Kiro
- **URL**: https://github.com/kirodotdev/Kiro/issues

### Search Scope
- Open Issues (unresolved issues)
- Closed Issues (resolved issues)
- Discussions (discussion area)

## Search Steps

### Step 1: Prepare Search Keywords

**Chinese to English Translation**:
```
Chinese question → Extract keywords → Translate to English
```

**Examples**:
- "如何配置 MCP" → "how to configure MCP"
- "插件安装失败" → "plugin installation failed"
- "性能问题" → "performance issue"

### Step 2: Use GitHub MCP Search

**Basic Search**:
```
Use github MCP's search_issues tool
Parameters:
  - repo: kirodotdev/Kiro
  - query: [English keywords]
  - state: all (search all states)
```

**Advanced Search**:
```
Add label filters:
  - label:bug (bug-related)
  - label:enhancement (feature enhancement)
  - label:documentation (documentation-related)
  - label:question (question consultation)
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

### Step 4: Verify Answer

**Checklist**:
- Is the solution applicable to the current version
- Is there official confirmation
- Has it been verified by multiple people
- Is there an updated solution

## Search Examples

### Example 1: Plugin Issue

**User Question**: Kiro IDE Python plugin not loading

**Search Process**:
```
1. Keywords: "python plugin not loading"
2. Use github MCP search
3. Filter: label:bug
4. View related Issues
5. Extract solution
```

**Output Format**:
```
Problem Description: Python plugin not loading

Solution:
1. Check Python version compatibility
2. Reinstall plugin
3. Clear cache: rm -rf ~/.kiro/cache
4. Restart Kiro IDE

Reference Documentation:
[1]: GitHub Issue #123 - Python plugin loading issue
[2]: Official Documentation - Plugin Troubleshooting
```

### Example 2: Configuration Issue

**User Question**: How to configure custom MCP server

**Search Process**:
```
1. Keywords: "custom MCP server configuration"
2. Search Issues and Discussions
3. Find configuration examples
4. Extract best practices
```

**Output Format**:
```
Problem Description: Configure custom MCP server

Solution:
1. Add configuration in .kiro/settings/mcp.json
2. Configuration format:
   {
     "mcpServers": {
       "custom-server": {
         "command": "path/to/server",
         "args": []
       }
     }
   }
3. Restart Kiro to apply configuration

Reference Documentation:
[1]: GitHub Discussion #456 - Custom MCP setup
[2]: Official Documentation - MCP Configuration Guide
```

## Search Tips

### Keyword Optimization
- Use specific error messages
- Include version numbers (if relevant)
- Use technical terms (in English)

### Filtering Tips
```
Search syntax:
  - is:issue (search Issues only)
  - is:open (search unresolved only)
  - is:closed (search resolved only)
  - label:bug (specific label)
  - author:username (specific author)
  - sort:updated (sort by update)
```

### Time Range
- Prioritize Issues from the last 6 months
- Old Issues may be outdated
- Note version changes

## No Results Handling

If GitHub search returns no results:

### 1. Expand Search Scope
```
- Search related repositories
- Search community forums
- Use web search
```

### 2. Suggest User to Create Issue
```
If it's a new issue, suggest user to:
1. Create a new Issue on GitHub
2. Provide detailed problem description
3. Include reproduction steps
4. Attach environment information
```

### 3. Provide Temporary Solution
```
Based on similar issues, provide possible solution ideas
Indicate this is an unverified solution
Suggest user to try cautiously
```

## Notes

1. **Language Conversion**: Accurately translate technical terms
2. **Version Compatibility**: Note Kiro version differences
3. **Answer Timeliness**: Prioritize using the latest solutions
4. **Official Confirmation**: Indicate if there's an official response
5. **Link References**: Provide specific Issue links
