# Kiro Knowledge Base Assistant Power

Automatically query Kiro IDE and CLI official documentation, community knowledge base, and GitHub Issues to provide accurate answers to your Kiro questions.

## Features

- 🔍 **Smart Query**: Automatically identify question type and select the best knowledge source
- 📚 **Multi-Source Integration**: Integrate official documentation, community knowledge base and GitHub Issue
- 🎯 **Structured Output**: Provide clear problem description, solution, and reference links
- 🌐 **Bilingual Support**: Support Chinese and English questions, automatically translate search keywords

## Knowledge Base Sources

### Kiro IDE

- [Troubleshooting Documentation](https://kiro.dev/docs/troubleshooting/)
- [Official Documentation](https://kiro.dev/docs/)
- [Book of Kiro](https://kiro-community.github.io/book-of-kiro/)

### Kiro CLI

- [CLI Official Documentation](https://kiro.dev/docs/cli/)
- [Book of Kiro](https://kiro-community.github.io/book-of-kiro/)

### GitHub

- [Kiro Issues](https://github.com/kirodotdev/Kiro/issues)

## Installation

### Prerequisites

Ensure the following MCP servers are configured:

1. **fetch** - Web content retrieval

   ```bash
   uvx mcp-server-fetch
   ```

2. **chrome-devtools** - Browser automation

   ```bash
   npx -y @executeautomation/chrome-mcp
   ```

3. **github** - GitHub API (requires Personal Access Token)
   ```bash
   uvx mcp-server-github
   ```
   Set environment variable: `GITHUB_PERSONAL_ACCESS_TOKEN`

### Install Power

1. Open Powers panel in Kiro
2. Click **Add power from Local Path**
3. Select this directory

## Usage

Simply ask questions in Kiro, and the Power will activate automatically:

```
"How to fix Kiro IDE Python plugin not loading?"
"How to use the kiro spec create command?"
"How to configure custom MCP servers in Kiro?"
```

## Output Format

```
Problem Description: [Your question]

Solution:
[Detailed solution steps]

Reference Documentation:
[1]: [Document title] - [Link]
[2]: [Document title] - [Link]
```

## Directory Structure

```
my-power/
├── POWER.md                          # Power configuration and main instructions
├── mcp.json                          # MCP server configuration
├── README.md                         # Documentation
└── steering/                         # Workflow guidance
    ├── kiro-ide-workflow.md         # IDE issue query workflow
    ├── kiro-cli-workflow.md         # CLI issue query workflow
    └── github-search-workflow.md    # GitHub search workflow
```

## Workflow

1. **Problem Analysis**: Identify if it's an IDE or CLI issue
2. **Knowledge Base Query**: Query official documentation and community resources by priority
3. **GitHub Search**: If no answer, search related Issues
4. **Web Search**: Finally supplement with search engines
5. **Format Output**: Provide structured answers and reference links

## Notes

- GitHub Issues are mostly in English, keywords will be automatically translated
- Ensure MCP servers are running properly
- Some documents may require login to access

## Contributing

Welcome to submit improvement suggestions and new knowledge sources!

## License

MIT
