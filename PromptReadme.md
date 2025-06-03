# Documentation Generation Prompt for Templates

Generate documentation files with the following structure:

## 1. README.md Structure

### Required Sections
- Brief introduction explaining the template's purpose
- Configuration section with key settings
- Required Parameters section listing all inputs
- Output Tables/Data section describing produced data
- Features section listing key capabilities
- Links section with relevant documentation URLs

### Example Format
```markdown
# [Template Name]

Brief introduction about the template's purpose.

## Configuration
- Key setting 1
- Key setting 2

### Required Parameters
- `parameter_1` - Description
- `parameter_2` - Description

## Output Data
- `output_1` - Description and contents
- `output_2` - Description and contents

## Features
- Feature 1
- Feature 2

## Links
- [Documentation](url)
- [Resources](url)
```

## 2. description.md Structure

### Required Sections
- Problem/Solution paragraph (what problem does this template solve?)
- Quick start example (how can users test it quickly?)

### Example Format
```markdown
# [Template Name]

Need to [solve this problem]? This template [provides this solution] by [doing X]. Perfect for [specific use case].

Get started in minutes: [simple example of usage with expected outcome].
```

### Key Differences from README.md
- Shorter and more focused
- Emphasizes business value
- Includes practical example
- Highlights key use case
- Avoids technical details
- Written from user perspective

## Documentation Guidelines

### Content Standards
- Use clear, concise language
- Focus on user-relevant information
- Avoid mentioning obvious dependencies
- Keep descriptions practical and actionable
- Include specific examples where helpful

### Formatting Rules
- Use proper markdown hierarchy
- Maintain consistent formatting
- Include relevant external links
- Use code blocks for technical elements

### Essential Information
- Template purpose and benefits
- Required inputs/parameters
- Output data structure
- Key features and capabilities
- External documentation links

### What to Avoid
- Platform-specific dependencies
- Overly technical details
- Redundant information
- Ambiguous descriptions

## Quality Checklist
- [ ] All required sections included
- [ ] Parameters accurately described
- [ ] Output data structure verified
- [ ] Links tested and working
- [ ] Language is clear and concise
- [ ] Format is consistent
- [ ] User perspective maintained