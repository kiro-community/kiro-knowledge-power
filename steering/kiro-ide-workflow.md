# Kiro IDE Issue Query Workflow

Follow this workflow when users ask Kiro IDE related questions.

## Knowledge Base Priority

### 1. Troubleshooting Documentation (Highest Priority)

**URL**: https://kiro.dev/docs/troubleshooting/

**Applicable Scenarios**:

- Plugin issues
- Installation issues
- Performance issues
- Error messages

**Query Method**:

```
Use fetch MCP to retrieve content
If fails, use chrome-devtools to open page
```

### 2. Official Documentation

**URL**: https://kiro.dev/docs/

**Applicable Scenarios**:

- Feature usage
- Configuration instructions
- API documentation
- Best practices

**Query Method**:

```
1. First try fetch to retrieve homepage
2. Based on question type, navigate to specific section
3. If fetch fails, use chrome-devtools
```

### 3. Book of Kiro (Community Knowledge Base)

**URL**: https://kiro-community.github.io/book-of-kiro/

**Applicable Scenarios**:

- Community experience
- Usage tips
- Common patterns
- Practical cases

**Query Method**:

```
Use fetch to retrieve relevant sections
```

## Query Steps

### Step 1: Analyze Question

- Extract keywords
- Determine question type (installation/configuration/usage/error)
- Identify priority knowledge base to query

### Step 2: Execute Query

```
1. Based on question type, select corresponding knowledge base
2. Use fetch MCP to retrieve content
3. If fetch fails:
   - Use chrome-devtools to open page
   - Use take_snapshot to get page content
4. Extract relevant information
```

### Step 3: Supplementary Query

If no answer found:

```
1. Use github MCP to search Issues
   - Repository: kirodotdev/Kiro
   - Search keywords (in English)
   - View open and closed issues
2. If still no answer, use fetch for web search
```

### Step 4: Organize Answer

Output in the following format:

```
Problem Description: [User's question]

Solution:
[Detailed solution steps, listed point by point]

Reference Documentation:
[1]: [Document title] - [Link]
[2]: [Document title] - [Link]
```

## Common Question Types

### Installation Issues

- Prioritize querying Troubleshooting
- Check system requirements
- View installation guide

### Plugin Issues

- Prioritize querying Troubleshooting
- Check plugin compatibility
- View GitHub Issues

### Feature Usage

- Prioritize querying official documentation
- View Book of Kiro examples
- Search community discussions

### Error Messages

- Prioritize querying Troubleshooting
- Search GitHub Issues (using error message as keywords)

## Notes

1. **Language Processing**: GitHub Issues are mostly in English, keywords need translation
2. **Version Information**: Note the version applicability of documentation
3. **Link Validity**: Ensure provided links are accessible
4. **Answer Completeness**: Provide complete solution steps, don't omit key information
