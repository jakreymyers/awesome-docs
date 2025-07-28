# Template: Product Requirements Document

>If you need more information about how to fill in this template, read the accompanying [Writing Guide: Product Requirements Document](./guide_product-requirements.md) file.
>
> This template includes writing instructions and boilerplate text that you can customize, use as-is, or completely replace with your own text. This text is indicated in {curly brackets}. Make sure you replace the placeholders with your own text.

## Goals and Background Context

{This section establishes the foundation for all requirements. If a Project Brief exists, reference and build upon it. If not, gather this foundational information here.}

### Goals

{List the specific desired outcomes this PRD will deliver if successful. Focus on measurable results and user/business benefits.}

- {Goal 1: Specific outcome the project will achieve}
- {Goal 2: Specific outcome the project will achieve}
- {Goal 3: Specific outcome the project will achieve}

### Background Context

{Provide 1-2 short paragraphs summarizing what problem this solves and why. Explain the current landscape and need without repeating the goals.}

{Background paragraph 1: What we learned from discovery that led to this PRD}

{Background paragraph 2: The current state and why this solution is needed now}

### Change Log

{Track document versions and changes to maintain transparency and communication}

| Date | Version | Description | Author |
|------|---------|-------------|---------|
| {MM/DD/YYYY} | {1.0} | {Initial draft} | {Author name} |
| {MM/DD/YYYY} | {1.1} | {Major changes description} | {Author name} |

## Requirements

{Define the specific functional and non-functional requirements that the solution must meet. Each requirement should be clear, testable, and traceable.}

### Functional Requirements

{List specific functional capabilities the system must provide. Each requirement should be numbered and clearly testable.}

1. **FR1:** {The system must capability description with specific, measurable criteria}
2. **FR2:** {The system must capability description with specific, measurable criteria}
3. **FR3:** {The system must capability description with specific, measurable criteria}
4. **FR4:** {Additional functional requirement}
5. **FR5:** {Additional functional requirement}

{Continue numbering as needed. Example: "FR6: The Todo List uses AI to detect and warn against potentially duplicate todo items that are worded differently."}

### Non-Functional Requirements

{List performance, security, usability, and other quality requirements. These define how the system should perform, not what it should do.}

1. **NFR1:** {Performance, security, or quality requirement with specific metrics}
2. **NFR2:** {Performance, security, or quality requirement with specific metrics}
3. **NFR3:** {Performance, security, or quality requirement with specific metrics}
4. **NFR4:** {Additional non-functional requirement}
5. **NFR5:** {Additional non-functional requirement}

{Continue numbering as needed. Example: "NFR1: AWS service usage must aim to stay within free-tier limits where feasible."}

## User Interface Design Goals

{Include this section if the PRD involves user interface requirements. This captures high-level UI/UX vision to guide design and development.}

### Overall UX Vision

{Describe the overall user experience philosophy and approach. What should using this product feel like?}

{High-level description of the intended user experience, interaction style, and usability goals}

### Key Interaction Paradigms

{Describe the primary ways users will interact with the system}

{Description of main interaction patterns, input methods, and user workflows}

### Core Screens and Views

{List the most critical screens or views from a product perspective. Focus on conceptual high-level views that deliver PRD value.}

- **{Screen/View Name}:** {Purpose and key functionality}
- **{Screen/View Name}:** {Purpose and key functionality}
- **{Screen/View Name}:** {Purpose and key functionality}

{Examples: "Login Screen", "Main Dashboard", "Item Detail Page", "Settings Page"}

### Accessibility Requirements

{Specify accessibility standards and requirements}

**Accessibility Level:** {None | WCAG AA | WCAG AAA | Custom Requirements}

{Describe specific accessibility requirements, standards compliance, or custom needs}

### Branding Guidelines

{Document any branding elements or style guides that must be incorporated}

{Description of branding requirements, style guides, visual identity constraints, or design system requirements}

{Example: "Replicate the look and feel of early 1900s black and white cinema, including animated effects replicating film damage or projector glitches during page or state transitions."}

### Target Platforms

**Device and Platform Support:** {Web Responsive | Mobile Only | Desktop Only | Cross-Platform}

{Provide specific details about supported devices, browsers, operating systems, and any platform-specific requirements}

{Examples: "Web Responsive, and all mobile platforms", "iPhone Only", "ASCII Windows Desktop"}

## Technical Assumptions

{Document technical decisions and constraints that will guide architecture and implementation. These become requirements for the technical team.}

### Repository Structure

**Repository Organization:** {Monorepo | Polyrepo | Multi-repo}

{Provide rationale for the repository structure choice and any specific organization requirements}

### Service Architecture

{CRITICAL DECISION - Document the high-level service architecture approach}

**Architecture Pattern:** {Monolith | Microservices | Serverless | Hybrid}

{Explain the architectural approach and rationale based on project goals, team capabilities, and requirements}

### Testing Requirements

{CRITICAL DECISION - Document testing strategy and requirements}

**Testing Scope:** {Unit Only | Unit + Integration | Full Testing Pyramid | Custom Approach}

{Describe the testing strategy, including unit tests, integration tests, end-to-end tests, and any manual testing requirements}

### Additional Technical Assumptions

{Document any other technical assumptions, constraints, or requirements discovered during PRD development}

- {Technical assumption 1 with rationale}
- {Technical assumption 2 with rationale}
- {Technical assumption 3 with rationale}

## Epic List

{Present a high-level list of all epics that organize the development work. Each epic should deliver significant, end-to-end functionality.}

{CRITICAL: Epics must be logically sequential following agile best practices. Each epic should deliver deployable, testable functionality that provides value.}

### Epic Overview

{Provide a brief explanation of the epic organization and sequencing rationale}

### Epic Definitions

1. **Epic 1: {Epic Title}**
   {One sentence goal statement describing the value this epic delivers}

2. **Epic 2: {Epic Title}**
   {One sentence goal statement describing the value this epic delivers}

3. **Epic 3: {Epic Title}**
   {One sentence goal statement describing the value this epic delivers}

4. **Epic 4: {Epic Title}**
   {One sentence goal statement describing the value this epic delivers}

{Examples:
- "Epic 1: Foundation & Core Infrastructure: Establish project setup, authentication, and basic user management"
- "Epic 2: Core Business Entities: Create and manage primary domain objects with CRUD operations"}

## Epic Details

{For each epic, provide expanded goals and detailed story breakdowns. Each epic should be reviewed as a complete unit.}

### Epic {Number}: {Epic Title}

{Expanded goal: 2-3 sentences describing the objective and value all stories in this epic will achieve}

#### Epic Goal Statement

{Detailed description of what this epic accomplishes and why it's valuable}

#### Stories

{CRITICAL: Stories must be logically sequential within the epic. Each story should be a "vertical slice" delivering complete functionality sized for AI agent execution (2-4 hours of focused work).}

##### Story {Epic Number}.{Story Number}: {Story Title}

**User Story:**
As a {user type},
I want {action or capability},
so that {benefit or value}.

**Acceptance Criteria:**
1. {Specific, testable criterion that defines "done"}
2. {Specific, testable criterion that defines "done"}
3. {Specific, testable criterion that defines "done"}
4. {Additional acceptance criteria as needed}

{Continue with additional stories in this epic, maintaining sequential numbering}

##### Story {Epic Number}.{Story Number}: {Story Title}

**User Story:**
As a {user type},
I want {action or capability},
so that {benefit or value}.

**Acceptance Criteria:**
1. {Specific, testable criterion that defines "done"}
2. {Specific, testable criterion that defines "done"}
3. {Specific, testable criterion that defines "done"}

{Repeat the Epic Details section for each epic defined in the Epic List}

## Checklist Results Report

{This section will contain the results of running quality assurance checklists against the PRD. Include this section to document validation and completeness.}

{Document the results of PRD quality checks, completeness validation, and stakeholder review outcomes}

## Next Steps

{Define the immediate actions and handoffs needed to begin implementation}

### Immediate Actions

1. {Action item with owner and timeline}
2. {Action item with owner and timeline}
3. {Action item with owner and timeline}

### UX Expert Handoff

{Brief prompt for UX expert to begin design work based on this PRD}

This PRD provides the complete functional and UI requirements for {Project Name}. Please begin UX design work focusing on the core screens and interaction paradigms defined in the UI Design Goals section.

### Architecture Team Handoff

{Brief prompt for technical architect to begin architecture design based on this PRD}

This PRD provides complete requirements and technical assumptions for {Project Name}. Please create detailed architecture documentation based on the technical assumptions and functional requirements specified in this document.

---
