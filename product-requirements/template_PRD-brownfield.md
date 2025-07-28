# Template: Brownfield Enhancement PRD

>If you need more information about how to fill in this template, read the accompanying [Writing Guide: Brownfield Enhancement PRD](./guide_brownfield-prd.md) file.
>
> This template includes writing instructions and boilerplate text that you can customize, use as-is, or completely replace with your own text. This text is indicated in {curly brackets}. Make sure you replace the placeholders with your own text.

## Project Analysis and Context

{IMPORTANT - SCOPE ASSESSMENT REQUIRED: This PRD is for SIGNIFICANT enhancements to existing projects that require comprehensive planning and multiple stories. For simple feature additions or bug fixes that could be completed in 1-2 focused development sessions, consider using simpler enhancement approaches instead. This full PRD process is designed for substantial enhancements that require architectural planning and multiple coordinated stories.}

{Gather comprehensive information about the existing project. This section must be completed before proceeding with requirements. Throughout this analysis, explicitly confirm your understanding with stakeholders before making recommendations.}

### Existing Project Overview

{Check if project analysis was already performed through documentation tools or IDE analysis}

#### Analysis Source

{Indicate one of the following sources for project information:}
- **Document Project Output:** {Available at specific path location}
- **IDE-Based Analysis:** {Fresh analysis performed in development environment}
- **User-Provided Information:** {Information gathered through stakeholder interviews}

#### Current Project State

{Provide a brief description of what the project currently does and its primary purpose}

{If document project output exists: Extract summary from existing technical documentation}
{Otherwise: Brief description of current functionality and core purpose}

### Available Documentation Analysis

{Document the existing project documentation and identify gaps}

#### Available Documentation

{Check all available documentation types:}

- [ ] Tech Stack Documentation
- [ ] Source Tree/Architecture Documentation
- [ ] Coding Standards and Guidelines
- [ ] API Documentation
- [ ] External API Documentation
- [ ] UX/UI Guidelines and Style Guides
- [ ] Technical Debt Documentation
- [ ] Other: {Specify additional documentation types}

{If critical documentation is missing, recommend completing project documentation before proceeding with enhancement planning}

### Enhancement Scope Definition

{Work with stakeholders to clearly define the type and scope of enhancement}

#### Enhancement Type

{Determine which type of enhancement this represents:}

- [ ] New Feature Addition
- [ ] Major Feature Modification
- [ ] Integration with New Systems
- [ ] Performance/Scalability Improvements
- [ ] UI/UX Overhaul
- [ ] Technology Stack Upgrade
- [ ] Bug Fix and Stability Improvements
- [ ] Other: {Specify enhancement type}

#### Enhancement Description

{Provide 2-3 sentences describing what will be added or changed in the existing system}

#### Impact Assessment

{Assess the scope of impact on existing codebase:}

- [ ] **Minimal Impact:** Isolated additions with no changes to existing code
- [ ] **Moderate Impact:** Some existing code changes required
- [ ] **Significant Impact:** Substantial existing code modifications needed
- [ ] **Major Impact:** Architectural changes and system-wide modifications required

### Goals and Background Context

#### Goals

{List the specific desired outcomes this enhancement will deliver if successful:}

- {Goal 1: Specific outcome the enhancement will achieve}
- {Goal 2: Specific outcome the enhancement will achieve}
- {Goal 3: Specific outcome the enhancement will achieve}

#### Background Context

{Provide 1-2 short paragraphs explaining why this enhancement is needed, what problem it solves, and how it fits with the existing project}

{Background paragraph 1: Current state and problem identification}

{Background paragraph 2: Why this enhancement is needed now and how it aligns with existing project goals}

### Change Log

{Track document versions and changes}

| Date | Version | Description | Author |
|------|---------|-------------|---------|
| {MM/DD/YYYY} | {1.0} | {Initial brownfield enhancement PRD} | {Author name} |
| {MM/DD/YYYY} | {1.1} | {Major changes description} | {Author name} |

## Requirements

{Draft functional and non-functional requirements based on validated understanding of the existing project. Confirm requirements align with the project's actual architecture and constraints.}

### Functional Requirements

{Define specific functional capabilities the enhancement must provide while maintaining existing functionality}

1. **FR1:** {The enhancement must capability description with specific, measurable criteria}
2. **FR2:** {The enhancement must capability description with specific, measurable criteria}
3. **FR3:** {The enhancement must capability description with specific, measurable criteria}
4. **FR4:** {Additional functional requirement}
5. **FR5:** {Additional functional requirement}

{Continue numbering as needed. Focus on new capabilities while ensuring existing functionality is preserved}

### Non-Functional Requirements

{Define performance, security, usability, and quality requirements that consider existing system constraints}

1. **NFR1:** {Performance, security, or quality requirement with specific metrics that align with existing system capabilities}
2. **NFR2:** {Performance, security, or quality requirement with specific metrics that align with existing system capabilities}
3. **NFR3:** {Performance, security, or quality requirement with specific metrics that align with existing system capabilities}
4. **NFR4:** {Additional non-functional requirement}
5. **NFR5:** {Additional non-functional requirement}

{Continue numbering as needed. Requirements should maintain or improve upon existing system performance}

### Compatibility Requirements

{Critical for brownfield projects - define what must remain compatible with existing systems}

1. **CR1:** {Existing API compatibility requirement and constraints}
2. **CR2:** {Database schema compatibility requirement and migration strategy}
3. **CR3:** {UI/UX consistency requirement with existing design patterns}
4. **CR4:** {Integration compatibility requirement with external systems}
5. **CR5:** {Additional compatibility requirement}

## User Interface Enhancement Goals

{Include this section if the enhancement involves UI changes}

### Integration with Existing UI

{Describe how new UI elements will fit with existing design patterns, style guides, and component libraries}

{Detail the approach for maintaining visual and interaction consistency with the existing application while introducing new functionality}

### Modified and New Screens

{List only the screens and views that will be modified or added by this enhancement}

**Modified Screens:**
- **{Screen Name}:** {Description of modifications and integration approach}
- **{Screen Name}:** {Description of modifications and integration approach}

**New Screens:**
- **{Screen Name}:** {Purpose and integration with existing navigation}
- **{Screen Name}:** {Purpose and integration with existing navigation}

### UI Consistency Requirements

{Define specific requirements for maintaining visual and interaction consistency}

- {Consistency requirement 1: Design system integration}
- {Consistency requirement 2: Component library usage}
- {Consistency requirement 3: Navigation pattern alignment}

## Technical Constraints and Integration Requirements

{Define detailed technical constraints based on existing project analysis}

### Existing Technology Stack

{Document the current technology stack and version constraints}

**Languages:** {Programming languages currently used with versions}

**Frameworks:** {Frontend and backend frameworks with versions}

**Database:** {Database systems and versions currently in use}

**Infrastructure:** {Hosting, deployment, and infrastructure technologies}

**External Dependencies:** {Third-party services and APIs currently integrated}

### Integration Approach

{Define how the enhancement will integrate with existing architecture}

**Database Integration Strategy:** {How database changes will be managed and integrated}

**API Integration Strategy:** {How new APIs will integrate with existing endpoints}

**Frontend Integration Strategy:** {How frontend changes will integrate with existing components}

**Testing Integration Strategy:** {How testing will ensure existing functionality remains intact}

### Code Organization and Standards

{Define how new code will fit existing patterns based on project analysis}

**File Structure Approach:** {How new files and directories will be organized}

**Naming Conventions:** {Existing naming patterns that must be followed}

**Coding Standards:** {Code quality and style standards from existing project}

**Documentation Standards:** {Documentation requirements and formats}

### Deployment and Operations

{Define how the enhancement fits existing deployment pipeline}

**Build Process Integration:** {How build processes will accommodate new code}

**Deployment Strategy:** {Deployment approach that minimizes risk to existing system}

**Monitoring and Logging:** {Integration with existing monitoring and logging systems}

**Configuration Management:** {How configuration changes will be managed}

### Risk Assessment and Mitigation

{Build risk assessment incorporating existing known issues and technical debt}

**Technical Risks:** {Risks related to code changes and technical implementation}

**Integration Risks:** {Risks related to integrating with existing systems}

**Deployment Risks:** {Risks related to deploying changes to production environment}

**Mitigation Strategies:** {Specific strategies to address identified risks}

## Epic and Story Structure

{For brownfield projects, typically favor a single comprehensive epic unless multiple unrelated enhancements are requested}

### Epic Approach

**Epic Structure Decision:** {Single epic | Multiple epics} with {rationale based on actual project analysis}

{Explain the rationale for epic structure - typically single epic for brownfield unless multiple unrelated features are being added}

## Epic Details

### Epic 1: {Enhancement Title}

{Comprehensive epic that delivers the brownfield enhancement while maintaining existing functionality}

**Epic Goal:** {What this epic will accomplish and the value it will deliver}

**Integration Requirements:** {Key integration points and compatibility requirements}

#### Story 1.1: {Story Title}

**User Story:**
As a {user type},
I want {action or capability},
so that {benefit or value}.

**Acceptance Criteria:**
1. {Specific, testable criterion that defines completion}
2. {Specific, testable criterion that defines completion}
3. {Specific, testable criterion that defines completion}
4. {Additional acceptance criteria as needed}

**Integration Verification:**
1. **IV1:** {Verification that existing functionality remains intact}
2. **IV2:** {Verification that integration points work correctly}
3. **IV3:** {Verification that performance impact is within acceptable limits}

#### Story 1.2: {Story Title}

{Follow the same structure for additional stories}

**User Story:**
As a {user type},
I want {action or capability},
so that {benefit or value}.

**Acceptance Criteria:**
1. {Specific, testable criterion that defines completion}
2. {Specific, testable criterion that defines completion}
3. {Specific, testable criterion that defines completion}

**Integration Verification:**
1. **IV1:** {Verification that existing functionality remains intact}
2. **IV2:** {Verification that integration points work correctly}
3. **IV3:** {Verification that performance impact is within acceptable limits}

{Continue with additional stories as needed. Stories must be logically sequential with clear dependencies. Each story should deliver value while maintaining system integrity. The sequence should minimize risk to existing system through incremental integration rather than big-bang changes.}

## Next Steps

{Define immediate actions needed to begin implementation}

### Immediate Actions

1. {Action item with owner and timeline}
2. {Action item with owner and timeline}
3. {Action item with owner and timeline}

### Architecture Review

{If architectural changes are required, define the review process}

This enhancement requires {architectural review | no architectural changes} based on the scope and impact assessment. {If review required: Architectural review should focus on integration points, compatibility requirements, and risk mitigation strategies.}

### Implementation Handoff

{Provide guidance for development team}

This Brownfield Enhancement PRD provides complete requirements and integration guidance for {Project Name}. The implementation team should prioritize maintaining existing functionality while delivering the specified enhancements. All changes should be implemented incrementally with thorough testing at each stage.

---
