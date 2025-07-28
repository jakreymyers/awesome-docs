# Template: Architecture - Brownfield

>If you need more information about how to fill in this template, read the accompanying [Writing Guide: Architecture](./guide_architecture.md) file.
>
> This template includes writing instructions and boilerplate text that you can customize, use as-is, or completely replace with your own text. This text is indicated in {curly brackets}. Make sure you replace the placeholders with your own text.

## Introduction

{IMPORTANT - SCOPE ASSESSMENT REQUIRED: This architecture document is for SIGNIFICANT enhancements to existing projects that require comprehensive architectural planning and integration analysis. For simple additions that don't require architectural changes, consider simpler enhancement approaches.}

{This document outlines the architectural approach for enhancing {Project Name} with new functionality while ensuring seamless integration with existing systems. It serves as the comprehensive blueprint for AI-driven development that maintains system stability while delivering new value.}

### Relationship to Existing Architecture

This document supplements and extends the existing project architecture by defining how new components integrate with current systems. Where conflicts arise between new and existing patterns, this document provides clear guidance for maintaining consistency while implementing enhancements.

Understanding the existing system is crucial for successful brownfield development. Unlike greenfield projects where you design optimal solutions, brownfield projects require working within existing constraints while maximizing enhancement value.

### Existing Project Analysis

{Conduct thorough analysis of the existing project before making architectural recommendations}

#### Current System Overview

**Project Purpose:** {What the existing project currently accomplishes}

**Current Architecture Style:** {Monolith/Microservices/Serverless/Hybrid}

**Technology Foundation:** {Core technologies, frameworks, and versions currently in use}

**Deployment Infrastructure:** {Current hosting, deployment processes, and infrastructure}

**System Scale:** {Current user base, data volume, performance characteristics}

#### Documentation Review

{Document what existing project information has been analyzed}

**Available Documentation:**
- {Documentation type 1: location and quality assessment}
- {Documentation type 2: location and quality assessment}
- {Documentation type 3: location and quality assessment}

**Documentation Gaps:** {Critical information missing from existing documentation}

#### System Constraints Analysis

{Identify limitations and constraints from the existing system}

**Technical Constraints:**
- {Constraint 1: description and impact on enhancement}
- {Constraint 2: description and impact on enhancement}
- {Constraint 3: description and impact on enhancement}

**Operational Constraints:**
- {Operational limitation 1: impact on new development}
- {Operational limitation 2: impact on new development}

**Business Constraints:**
- {Business constraint 1: impact on enhancement approach}
- {Business constraint 2: impact on enhancement approach}

### Change Log

{Track architectural decisions and document evolution}

| Date | Version | Description | Author |
|------|---------|-------------|--------|
| {MM/DD/YYYY} | {1.0} | {Initial brownfield architecture analysis} | {Author name} |
| {MM/DD/YYYY} | {1.1} | {Enhancement architecture decisions} | {Author name} |

## Enhancement Scope and Integration Strategy

{Define the enhancement scope and how it integrates with existing systems based on validated analysis}

### Enhancement Overview

**Enhancement Type:** {New feature addition | Major feature modification | System integration | Performance improvement | UI/UX modernization | Technology stack upgrade}

**Enhancement Scope:** {Comprehensive description of what will be added, changed, or improved}

**Integration Complexity:** {Minimal | Moderate | Significant | Major impact on existing architecture}

**Success Criteria:** {How success will be measured for this enhancement}

### Integration Architecture Strategy

The integration approach balances delivering new value with maintaining existing system stability. This requires careful coordination between new and existing components, data structures, and user workflows.

**Code Integration Approach:** {How new code will integrate with existing patterns, conventions, and architecture}

**Data Integration Strategy:** {How new data structures will integrate with existing schemas and data flows}

**API Integration Method:** {How new APIs will work with existing endpoints while maintaining backward compatibility}

**User Experience Integration:** {How enhanced functionality will integrate with existing user interfaces and workflows}

### Compatibility Requirements

**Existing API Preservation:** {Requirements for maintaining current API functionality and contracts}

**Database Compatibility:** {Requirements for maintaining existing data structures and relationships}

**User Workflow Continuity:** {Requirements for preserving familiar user interaction patterns}

**Performance Impact Limits:** {Acceptable performance impact ranges and improvement requirements}

**Integration Testing Requirements:** {Specific testing needed to verify compatibility}

## Technology Stack Analysis and Alignment

{Ensure enhancement technologies align with existing stack while identifying necessary additions}

### Current Technology Assessment

{Document existing technologies that must be maintained or integrated with}

| Category | Current Technology | Version | Enhancement Usage | Integration Notes |
|----------|-------------------|---------|-------------------|-------------------|
| **Programming Language** | {Language} | {Version} | {How enhancement will use this} | {Compatibility considerations} |
| **Framework** | {Framework} | {Version} | {Integration approach} | {Version constraints or upgrades} |
| **Database** | {Database} | {Version} | {Data integration method} | {Schema change requirements} |
| **Authentication** | {Auth system} | {Version} | {Auth integration approach} | {User session compatibility} |
| **Frontend Framework** | {Frontend tech} | {Version} | {UI integration method} | {Component compatibility} |

### New Technology Additions

{Include only technologies that are absolutely required and cannot be avoided}

| Technology | Version | Purpose | Rationale | Integration Strategy |
|------------|---------|---------|-----------|---------------------|
| {New Technology 1} | {Version} | {Specific purpose} | {Why existing stack can't handle this} | {How it integrates with existing} |
| {New Technology 2} | {Version} | {Specific purpose} | {Why this is necessary} | {Integration and compatibility approach} |

### Technology Risk Assessment

**Integration Risks:** {Risks related to technology integration and compatibility}

**Upgrade Requirements:** {Existing technology upgrades needed for compatibility}

**Alternative Approaches:** {Alternative technology choices considered and why they were rejected}

## Data Architecture Integration

{Define how new data structures integrate with existing data models and flows}

### Enhanced Data Models

#### {New Model Name}

**Purpose:** {What this new model represents and its role in the enhancement}

**Integration Points:** {How this model integrates with existing data structures}

**Key Attributes:**
- {attribute_name}: {data_type} - {description and relationship to existing data}
- {attribute_name}: {data_type} - {description and constraints}
- {attribute_name}: {data_type} - {description and validation rules}

**Relationships:**
- **To Existing Models:** {Relationships with current data structures}
- **To New Models:** {Relationships with other new models}

**Migration Strategy:** {How existing data will be handled during enhancement implementation}

#### {Additional New Model}

{Follow the same structure for other new data models}

### Database Integration Strategy

**Schema Evolution Approach:** {How database schema will be enhanced while maintaining compatibility}

**Data Migration Plan:**
- **New Tables:** {List and purpose of new tables}
- **Modified Tables:** {Existing tables requiring changes and modification strategy}
- **Data Transformation:** {How existing data will be transformed or preserved}
- **Rollback Strategy:** {How changes can be reversed if necessary}

**Backward Compatibility Measures:**
- {Compatibility measure 1: ensuring existing queries continue working}
- {Compatibility measure 2: maintaining existing data access patterns}
- {Compatibility measure 3: preserving existing API data contracts}

**Performance Impact Assessment:** {Expected impact on existing database performance and mitigation strategies}

## Component Architecture Enhancement

{Define new components and their integration with existing system architecture}

### Integration Architecture Overview

{Describe how new components fit within the existing system architecture}

```mermaid
graph TD
    A[{Existing Frontend}] --> B[{Enhanced API Layer}]
    B --> C[{Existing Business Logic}]
    B --> D[{New Enhancement Logic}]
    C --> E[{Existing Database}]
    D --> E
    D --> F[{New Data Store}]
    D --> G[{External Integration}]
```

### Enhanced Components

#### {New Component Name}

**Responsibility:** {What this component handles and its primary purpose in the enhancement}

**Integration Strategy:** {How this component interfaces with existing system components}

**Key Interfaces:**
- **To Existing Systems:** {APIs or contracts with existing components}
- **New Interfaces:** {New APIs or contracts this component provides}

**Dependencies:**
- **Existing System Dependencies:** {Dependencies on current system components}
- **New Dependencies:** {Dependencies on other new components or external services}

**Technology Alignment:** {How component technology choices align with existing stack}

**Error Handling Integration:** {How component errors integrate with existing error handling}

#### {Additional New Component}

{Follow the same structure for other new components}

### Existing Component Modifications

#### {Modified Existing Component}

**Current Functionality:** {Brief description of existing component responsibilities}

**Enhancement Modifications:** {Specific changes required for enhancement integration}

**Compatibility Preservation:** {How existing functionality will be preserved}

**Migration Strategy:** {How modifications will be implemented without disrupting existing functionality}

**Testing Requirements:** {Specific testing needed to verify existing functionality remains intact}

## API Integration and Evolution

{Include this section if enhancement requires API changes or additions}

### API Integration Strategy

The API integration approach ensures new functionality extends existing API patterns while maintaining backward compatibility for current consumers. This requires careful versioning and gradual transition strategies.

**API Evolution Approach:** {How new APIs will extend existing API architecture}

**Versioning Strategy:** {How API versioning will handle new functionality}

**Authentication Integration:** {How new endpoints will integrate with existing authentication}

**Error Handling Consistency:** {How new API errors will align with existing error patterns}

### Enhanced API Endpoints

#### {New Endpoint Name}

**Method:** {HTTP method}

**Endpoint:** {API endpoint path}

**Purpose:** {What this endpoint accomplishes in the enhancement}

**Integration:** {How it relates to existing API structure}

**Authentication:** {Authentication requirements and integration}

**Request Format:**

```json
{
  "new_field_1": "value_type",
  "existing_compatible_field": "value_type",
  "enhancement_specific_field": "value_type"
}
```

**Response Format:**

```json
{
  "enhanced_data": "value_type",
  "backward_compatible_field": "value_type",
  "new_functionality_result": "value_type"
}
```

**Backward Compatibility:** {How this endpoint maintains compatibility with existing system expectations}

#### {Additional New Endpoint}

{Follow the same structure for additional API endpoints}

### Existing API Modifications

#### {Modified Existing Endpoint}

**Current Functionality:** {What the existing endpoint currently provides}

**Enhancement Modifications:** {Changes needed for enhancement integration}

**Compatibility Strategy:** {How existing consumers will be protected from breaking changes}

**Migration Path:** {How consumers can adopt enhanced functionality}

## External Integration Enhancement

{Include this section if enhancement requires new external API integrations}

### New External Dependencies

#### {External Service Name}

**Purpose:** {What this external service provides for the enhancement}

**Integration Method:** {How it integrates with existing external service patterns}

**Authentication:** {Authentication method and credential management}

**Error Handling:** {How external service errors integrate with existing error handling}

**Fallback Strategy:** {How system behaves if external service is unavailable}

**Existing System Impact:** {How this integration affects existing system behavior}

**Key Integration Points:**
- `{METHOD} {endpoint}` - {Purpose and integration with enhancement}
- `{METHOD} {endpoint}` - {Purpose and data flow}

**Monitoring Integration:** {How external service monitoring integrates with existing monitoring}

#### {Additional External Service}

{Follow the same structure for additional external integrations}

### External Service Risk Assessment

**Service Availability Impact:** {How external service downtime affects existing system}

**Data Privacy Considerations:** {How external services handle existing system data}

**Performance Impact:** {Expected impact on existing system performance}

**Alternative Solutions:** {Backup plans if external services become unavailable}

## Infrastructure Integration

{Define how enhancement infrastructure integrates with existing deployment and operations}

### Current Infrastructure Assessment

**Existing Deployment Architecture:** {Current hosting, deployment, and infrastructure setup}

**Infrastructure Tools:** {Current infrastructure management and deployment tools}

**Environment Structure:** {Existing development, staging, and production environments}

**Monitoring and Operations:** {Current monitoring, logging, and operational procedures}

### Enhancement Infrastructure Strategy

**Infrastructure Enhancement Approach:** {How new infrastructure needs will be addressed}

**Deployment Integration:** {How enhanced functionality will be deployed alongside existing system}

**Environment Compatibility:** {How enhancement will work across existing environments}

**Resource Requirements:** {Additional infrastructure resources needed for enhancement}

### Deployment Strategy

**Deployment Method:** {How enhancement will be deployed without disrupting existing system}

**Risk Mitigation:** {Strategies to minimize deployment risk to existing functionality}

**Rollback Procedures:** {How to quickly revert enhancement if issues arise}

**Monitoring Integration:** {How enhancement monitoring integrates with existing monitoring}

**Performance Impact Management:** {How to monitor and manage enhancement performance impact}

## Security Integration

{Ensure security consistency with existing system while addressing new security requirements}

### Existing Security Assessment

**Current Authentication:** {Existing user authentication mechanisms and patterns}

**Authorization Systems:** {Current permission and access control systems}

**Data Protection Measures:** {Current data encryption and protection approaches}

**Security Monitoring:** {Existing security monitoring and incident response}

**Compliance Requirements:** {Current regulatory compliance and audit requirements}

### Enhancement Security Integration

**Authentication Enhancement:** {How new functionality integrates with existing authentication}

**Authorization Extensions:** {How new permissions integrate with existing access control}

**Data Protection Integration:** {How enhancement data protection aligns with existing measures}

**Security Testing Requirements:** {Security testing needed for enhancement integration}

**Compliance Impact:** {How enhancement affects existing compliance requirements}

### Security Risk Assessment

**Integration Security Risks:** {Security risks specific to integrating with existing systems}

**Data Flow Security:** {Security considerations for new data flows between systems}

**Authentication Vulnerabilities:** {Potential authentication issues from enhancement}

**Mitigation Strategies:** {Specific strategies to address identified security risks}

## Testing Strategy for Brownfield Enhancement

{Define comprehensive testing approach that validates both new functionality and existing system integrity}

### Integration Testing Philosophy

Testing brownfield enhancements requires validating that new functionality works correctly while ensuring existing functionality remains unaffected. This dual focus makes testing strategy more complex than greenfield projects.

### Existing System Regression Testing

**Regression Test Strategy:** {How to verify existing functionality remains intact}

**Automated Regression Suite:** {Automated tests that verify existing system behavior}

**Performance Regression Testing:** {Testing to ensure enhancement doesn't degrade existing performance}

**User Workflow Testing:** {Testing existing user workflows continue working}

### Enhancement Testing Framework

**New Functionality Testing:** {Testing approach for new enhancement features}

**Integration Point Testing:** {Testing connections between new and existing components}

**Data Integrity Testing:** {Testing data consistency between new and existing systems}

**API Compatibility Testing:** {Testing API backward compatibility and new functionality}

### Testing Environment Strategy

**Test Data Management:** {How test data will handle both existing and new functionality}

**Environment Consistency:** {Ensuring test environments reflect production integration complexity}

**Testing Isolation:** {How to test enhancements without affecting existing system testing}

## Risk Assessment and Mitigation

{Identify and address risks specific to brownfield enhancement}

### Integration Risks

**Technical Integration Risks:**
- {Risk 1: Description, probability, impact, and specific mitigation strategy}
- {Risk 2: Description, probability, impact, and specific mitigation strategy}
- {Risk 3: Description, probability, impact, and specific mitigation strategy}

**User Impact Risks:**
- {User risk 1: Description and mitigation approach}
- {User risk 2: Description and mitigation approach}

**Data Migration Risks:**
- {Data risk 1: Description and protection strategy}
- {Data risk 2: Description and recovery approach}

### Operational Risks

**Deployment Risks:** {Risks related to deploying enhancement to production environment}

**Performance Risks:** {Risks of enhancement affecting existing system performance}

**Monitoring and Support Risks:** {Risks related to supporting enhanced system}

**Rollback Risks:** {Risks and limitations of rollback procedures}

### Risk Mitigation Strategy

**Staged Rollout Approach:** {How enhancement will be gradually deployed to minimize risk}

**Monitoring and Alerting:** {Enhanced monitoring to detect issues early}

**Contingency Planning:** {Specific plans for various failure scenarios}

**Team Readiness:** {How team will be prepared for enhancement support}

## Implementation Roadmap

{Define the specific phases and approach for implementing brownfield enhancement}

### Implementation Philosophy

Brownfield enhancement implementation prioritizes maintaining existing system stability while delivering new value. This requires careful sequencing, thorough testing, and gradual rollout strategies.

### Implementation Phases

**Phase 1: Foundation and Compatibility** {Duration: timeline}
- {Deliverable 1: Description and validation criteria}
- {Deliverable 2: Description and integration verification}
- {Validation checkpoint: Existing system functionality verification}

**Phase 2: Core Enhancement Implementation** {Duration: timeline}
- {Deliverable 1: Description and testing requirements}
- {Deliverable 2: Description and integration testing}
- {Validation checkpoint: New functionality and compatibility verification}

**Phase 3: Integration and Optimization** {Duration: timeline}
- {Deliverable 1: Description and performance validation}
- {Deliverable 2: Description and user acceptance testing}
- {Final validation: Full system integration verification}

### Success Criteria

**Technical Success Criteria:**
- {Criterion 1: Measurable technical outcome}
- {Criterion 2: Measurable integration outcome}
- {Criterion 3: Measurable performance outcome}

**Business Success Criteria:**
- {Criterion 1: Measurable business outcome}
- {Criterion 2: Measurable user outcome}

**Integration Success Criteria:**
- {Criterion 1: Compatibility verification}
- {Criterion 2: System stability verification}

## Next Steps and Team Handoff

{Define immediate actions and handoff guidance for implementation teams}

### Immediate Implementation Actions

1. {Action 1: Description, owner, and timeline}
2. {Action 2: Description, owner, and timeline}
3. {Action 3: Description, owner, and timeline}

### Development Team Handoff

This Brownfield Architecture Document provides the comprehensive technical blueprint for enhancing {Project Name} while maintaining existing system integrity. All architectural decisions are based on thorough analysis of the existing system and validated compatibility requirements.

**Implementation Priorities:**
1. {Priority 1: Focus area and rationale}
2. {Priority 2: Focus area and rationale}
3. {Priority 3: Focus area and rationale}

**Critical Integration Points:** {Key areas requiring special attention during implementation}

**Validation Requirements:** {How to verify implementation follows architecture and maintains compatibility}

### Architecture Review and Change Management

**Review Requirements:** {When architectural reviews are required during implementation}

**Change Management Process:** {How to handle architectural changes discovered during implementation}

**Documentation Updates:** {How this document will be maintained as implementation progresses}

**Stakeholder Communication:** {How architectural changes will be communicated to stakeholders}

---
