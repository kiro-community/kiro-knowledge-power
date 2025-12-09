# Kiro CLI Issue Query Workflow

Follow this workflow when users ask Kiro CLI related questions.

## Knowledge Base Priority

### 1. CLI Official Documentation (Highest Priority)

**URL**: https://kiro.dev/docs/cli/

**Applicable Scenarios**:

- CLI command usage
- Parameter descriptions
- Configuration files
- Workflows

**Query Method**:

```
1. Use fetch MCP to retrieve documentation
2. If fails, use chrome-devtools to open page
3. Navigate to specific command section
```

### 2. Book of Kiro (Community Knowledge Base)

**URL**: https://kiro-community.github.io/book-of-kiro/

**Applicable Scenarios**:

- CLI usage tips
- Automation scripts
- CI/CD integration
- Practical cases

**Query Method**:

```
Use fetch to retrieve relevant sections
Search CLI-related content
```

## Query Steps

### Step 1: Analyze Question

- Identify specific CLI command
- Determine question type (installation/configuration/usage/error)
- Extract key parameters and options

### Step 2: Execute Query

```
1. Query CLI official documentation
   - Use fetch to retrieve command documentation
   - Find relevant parameter descriptions

2. If documentation is not detailed enough:
   - Query Book of Kiro examples
   - Search community use cases

```

### Step 3: Supplementary Query

If no answer found:

```
1. Use github MCP to search Issues
   - Repository: kirodotdev/Kiro
   - Search: "cli" + [question keywords]
   - View related Issues and Discussions

2. If still no answer:
   - Use fetch for web search
   - Search: "kiro cli" + [problem description]
```

### Step 4: Organize Answer

Output in the following format:

```
Problem Description: [User's question]

Solution:
[Command example]
[Parameter description]
[Usage steps]

Reference Documentation:
[1]: [Document title] - [Link]
[2]: [Document title] - [Link]
```

## Common CLI Question Types

### Command Usage

**Example**: How to use the `kiro spec` command?

**Query Process**:

1. Query official documentation command reference
2. View Book of Kiro usage examples
3. Provide complete command format and parameter descriptions

### Configuration Issues

**Example**: How to configure CLI default settings?

**Query Process**:

1. Query official documentation configuration section
2. View configuration file format
3. Provide configuration examples

### Integration Issues

**Example**: How to use Kiro CLI in CI/CD?

**Query Process**:

1. Query Book of Kiro integration cases
2. Search GitHub Issues for related discussions
3. Provide complete integration examples

### Error Troubleshooting

**Example**: CLI command execution failed

**Query Process**:

1. Analyze error message
2. Search GitHub Issues (using error message)
3. Provide troubleshooting steps and solutions

## Output Format Example

```
Problem Description: How to use kiro spec create command to create a new spec?

Solution:
1. Basic command format:
   kiro spec create <spec-name> [options]

2. Common parameters:
   --template: Specify template
   --output: Specify output directory

3. Usage example:
   kiro spec create my-feature --template=basic

4. After execution, a spec file will be created in the current directory

Reference Documentation:
[1]: Kiro CLI Command Reference - https://kiro.dev/docs/cli/commands
[2]: Book of Kiro - Spec Creation Guide - https://kiro-community.github.io/book-of-kiro/specs
```

## Notes

1. **Command Format**: Use code blocks to display commands, ensure correct format
2. **Parameter Description**: Explain the purpose of each parameter in detail
3. **Complete Examples**: Provide complete examples that can be run directly
4. **Version Compatibility**: Note CLI version differences
5. **Environment Requirements**: Explain necessary environment configuration
