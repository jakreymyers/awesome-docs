# Template Collection Reference Guide

This reference guide provides comprehensive information about the documentation templates in this collection and their supporting files. Use this guide to understand the template structure, locate specific information, and implement templates effectively in your projects.

## Quick Reference

### Template File Types

| File Type | Filename Pattern | Purpose | When to Use |
|-----------|------------------|---------|-------------|
| **Template** | `template_[type].md` | Raw template with structure and embedded tips | Starting point for new documentation |
| **Writing Guide** | `guide_[type].md` | Detailed usage instructions and decision guidance | Need help filling sections or customizing |
| **Best Practices** | `practices_[type].md` | Workflow guidance for research, writing, maintenance | Want comprehensive process guidance |
| **Resources** | `resources_[type].md` | Examples, sources, and research references | Need examples or want to understand template design |

### Template Categories

| Category | Templates Available | Complexity |
|----------|-------------------|------------|
| **Product Planning** | Product Requirements (PRD), Architecture, Market Research | High |
| **User Documentation** | API Getting Started, Installation Guide, Quickstart, Tutorial, How-to | Medium |
| **Reference Documentation** | API Reference, Glossary, Style Guide, Terminology System | Medium |
| **Project Documentation** | README, Changelog, Release Notes, Troubleshooting | Low-Medium |
| **Research & Analysis** | Concept, User Personas, Competitor Analysis, Brainstorming Report | Medium |
| **Technical Specifications** | Frontend Specification, Bug Report, User Story | Low-Medium |

## How to Use This Reference Guide

### Finding the Right Template

1. **Identify your documentation type** using the Template Categories table above
2. **Check template complexity** to understand the scope of supporting files available
3. **Locate the template directory** in the collection (each template has its own folder)
4. **Start with the template file** (`template_[type].md`) for immediate use
5. **Consult the writing guide** (`guide_[type].md`) for detailed guidance

### Understanding File Purposes

The template collection provides different levels of support depending on your needs and experience level. For quick implementation, the template file alone may be sufficient. The template files include embedded guidance within curly brackets that you can follow directly.

When you need more comprehensive support, the writing guide explains the purpose of each section and provides decision-making guidance for complex scenarios. These guides often include examples and decision trees to help you choose the right approach for your specific situation.

Teams establishing documentation processes benefit from the best practices files, which cover the complete lifecycle from research through maintenance. The resources files provide real-world examples and explain the research foundation behind template decisions.

## Template File Reference

### Template Files (`template_[type].md`)

**Purpose**: Structured starting point for creating documentation

**Structure**:
- **Document title** (Heading 1)
- **Introductory guidance** in {curly brackets} directing to writing guide
- **Content sections** (Heading 2) with embedded tips in {curly brackets}
- **Placeholder content** showing expected information types

**Usage Guidelines**:
- Copy the template file as your starting document
- Replace all content in {curly brackets} with your specific information
- Remove or modify sections based on your needs
- Use heading 3 for sub-sections when needed (avoid going deeper than level 3)

**Customization**:
- All sections are customizable - add, remove, or modify as needed
- Embedded tips provide guidance but can be replaced with your content
- Structure serves as a foundation, not a rigid requirement

## Writing Guide Reference

### Writing Guide Files (`guide_[type].md`)

**Purpose**: Comprehensive instructions for effective template usage

**Standard Structure**:
- **"Why do I need this type of document?"** - Purpose and value explanation
- **Template selection guidance** (for templates with multiple variants)
- **Section-by-section guidance** - Detailed instructions for each template section
- **Best practices** - Key principles for this documentation type
- **Common pitfalls** - Mistakes to avoid and how to prevent them

**When to Consult**:
- Before starting complex templates
- When unsure about section content or purpose
- For guidance on optional vs. required sections
- When customizing templates for specific organizational needs

**Navigation Tips**:
- Use the table of contents to jump to specific sections
- Section headings match template section names for easy cross-reference
- Look for decision trees and selection matrices for complex choices

## Best Practices Reference

### Best Practices Files (`practices_[type].md`)

**Purpose**: Complete workflow guidance for documentation lifecycle

**Standard Structure**:
- **Before writing** - Research and preparation strategies
- **Writing process** - Specific techniques for this content type
- **Maintenance practices** - Keeping documentation current and effective
- **Quality assurance** - Validation and review approaches

**When to Use**:
- Setting up documentation processes for teams
- Improving quality and consistency of existing documentation
- Understanding the complete lifecycle of this content type
- Training team members on documentation best practices

**Process Integration**:
- Complements template and guide files with workflow context
- Provides broader perspective beyond individual document creation
- Includes maintenance and evolution strategies often overlooked

## Resources Reference

### Resources Files (`resources_[type].md`)

**Purpose**: Examples, research sources, and design rationale

**Standard Structure**:
- **Examples section** - High-quality real-world implementations with analysis
- **Sources consulted** - Research materials and references used in template design
- **Design rationale** - Explanation of template decisions and alternatives considered

**When to Reference**:
- Seeking inspiration from excellent examples
- Understanding the research behind template design
- Customizing templates for specific organizational contexts
- Maintaining or updating existing templates

**Value for Different Users**:

| User Type | Primary Benefit |
|-----------|----------------|
| **Template users** | Real-world examples and implementation patterns |
| **Template customizers** | Understanding of design decisions enabling informed modifications |
| **Template maintainers** | Research foundation for evaluating future changes |
| **Quality reviewers** | Benchmarks for evaluating documentation effectiveness |

## Implementation Patterns

### Single Template Implementation

1. **Choose template** based on documentation needs
2. **Copy template file** as starting point
3. **Reference writing guide** for section-specific guidance
4. **Fill in template** replacing placeholder content
5. **Review against examples** in resources file (if available)

### Team Implementation

1. **Review best practices** for process establishment
2. **Customize templates** based on organizational needs using guide recommendations
3. **Establish review process** using quality criteria from best practices
4. **Create team guidelines** referencing relevant sections of guides
5. **Set up maintenance schedule** based on best practices recommendations

### Template Customization

1. **Study existing template** structure and embedded guidance
2. **Review writing guide** for understanding of section purposes
3. **Examine resources** for design rationale and alternative approaches
4. **Modify template** based on specific organizational requirements
5. **Update guidance** to reflect customizations for team use

## Template Collection Maintenance

### File Naming Conventions

- **Templates**: `template_[content-type].md`
- **Writing Guides**: `guide_[content-type].md`
- **Best Practices**: `practices_[content-type].md`
- **Resources**: `resources_[content-type].md`

### Content Standards

- **Consistency**: All files follow established patterns for structure and formatting
- **Cross-references**: Guides reference template sections; resources link to examples
- **Accessibility**: Clear headings, logical flow, and scannable organization
- **Completeness**: Each file type serves distinct purpose without unnecessary overlap

### Quality Indicators

- **Template usability**: Can be used effectively with minimal external guidance
- **Guide clarity**: Provides clear direction for decision-making and content creation
- **Process completeness**: Covers full lifecycle from research through maintenance
- **Resource relevance**: Examples and sources directly support template implementation

## Getting Help

### Troubleshooting Template Issues

1. **Check the writing guide** for section-specific guidance
2. **Review examples** in resources files for implementation patterns
3. **Consult best practices** for process and quality guidance
4. **Compare with similar templates** for alternative approaches

### Contributing Improvements

1. **Document specific issues** encountered during template use
2. **Propose solutions** based on best practices and resource research
3. **Test improvements** with actual documentation projects
4. **Update relevant files** (template, guide, resources, or best practices as appropriate)

---

This reference guide provides the foundation for effective use of the template collection. For specific implementation guidance, always consult the individual template files and their accompanying writing guides.
