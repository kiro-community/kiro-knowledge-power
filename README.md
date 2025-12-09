# Kiro Knowledge Base Assistant Power

Automatically query Kiro IDE and CLI official documentation, community knowledge base, and GitHub Issues to provide accurate answers to your Kiro questions.

## Features

- 🔍 **Smart Query**: Automatically identify question type and select the best knowledge source
- 📚 **Multi-Source Integration**: Integrate official documentation, community knowledge base and GitHub Issue
- 🎯 **Structured Output**: Provide clear problem description, solution, and reference links
- 🌐 **Bilingual Support**: Support Chinese and English questions, automatically translate search keywords

## Installation

### Prerequisites

Set environment variable:

- `GITHUB_PERSONAL_ACCESS_TOKEN`

### Install Power

1. Open Powers panel in Kiro
2. Click **Add Custom Power** -> **Import power from GitHub**
3. Enter this repository's URL: `https://github.com/kiro-community/kiro-knowledge-power`

## Usage

Simply ask questions in Kiro, and the Power will activate automatically:

```
"How to fix Kiro IDE Python plugin not loading?"
"How to use the kiro spec create command?"
"How to configure custom MCP servers in Kiro?"
```

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

## Contributing

Welcome to submit improvement suggestions and new knowledge sources!

## License

MIT
