# Template: Architecture - Greenfield

>If you need more information about how to fill in this template, read the accompanying [Writing Guide: Architecture](./guide_architecture.md) file.
>
> This template includes writing instructions and boilerplate text that you can customize, use as-is, or completely replace with your own text. This text is indicated in {curly brackets}. Make sure you replace the placeholders with your own text.

## Introduction

{This document outlines the complete architecture for {Project Name}, serving as the authoritative technical blueprint for AI-driven development. It ensures consistency across the entire technology stack and provides clear guidance for implementation decisions.}

{This template is designed for greenfield projects where you have complete freedom to choose optimal technologies and patterns. Sections are organized to support frontend-only, backend-only, or full-stack development by including or removing relevant sections as needed.}

### Project Foundation

{Document whether this project uses an existing foundation or starts completely from scratch}

**Project Type:** {Greenfield | Based on starter template | Clean slate}

{If using a starter template:}

**Template/Framework Name:** {Name and version of starter template or framework}

**Documentation:** {Link to template documentation or framework guides}

**Pre-configured Elements:**
- **Technology Stack:** {List pre-configured technologies and versions}
- **Project Structure:** {Describe existing organization patterns}
- **Development Tools:** {List included scripts, build tools, development tools}
- **Architectural Patterns:** {Note existing architectural decisions}
- **Constraints:** {Document any limitations imposed by the foundation}

### Change Log

{Track architectural decisions and document evolution}

| Date | Version | Description | Author |
|------|---------|-------------|--------|
| {MM/DD/YYYY} | {1.0} | {Initial architecture draft} | {Author name} |
| {MM/DD/YYYY} | {1.1} | {Major architectural changes} | {Author name} |

## High Level Architecture

{Provide a comprehensive overview of the system architecture that's understandable by both technical and non-technical stakeholders}

### Technical Summary

{Provide a 3-4 paragraph executive summary covering architectural style, technology choices, deployment approach, and how the architecture achieves project goals}

{Paragraph 1: Overall architectural approach and primary patterns}

{Paragraph 2: Technology stack selection and integration strategy}

{Paragraph 3: Deployment and infrastructure approach}

{Paragraph 4: How this architecture achieves project requirements and goals}

### Architecture Style and Patterns

**Primary Architecture Pattern:** {Monolithic | Microservices | Serverless | Jamstack | Hybrid}

**Pattern Rationale:** {Why this architectural pattern was chosen for the project}

**Design Principles:**
- {Design principle 1: explanation and application}
- {Design principle 2: explanation and application}
- {Design principle 3: explanation and application}

**Cross-Cutting Concerns:**
- **Logging:** {Logging strategy and implementation approach}
- **Security:** {Security approach and implementation strategy}
- **Error Handling:** {Error handling patterns and monitoring}
- **Configuration:** {Configuration management approach}

### System Context Diagram

{Include a high-level diagram showing the system in its environment}

```mermaid
graph TD
    A[{Users/Clients}] --> B[{Load Balancer/CDN}]
    B --> C[{Frontend Application}]
    C --> D[{API Gateway}]
    D --> E[{Backend Services}]
    E --> F[{Database}]
    E --> G[{External APIs}]
    E --> H[{File Storage}]
```

{Explain the key components, data flows, and integration points shown in the diagram}

## Tech Stack

{Define the complete technology stack with versions, purposes, and rationale - this is the single source of truth for all technology decisions}

### Core Technology Stack

| Category | Technology | Version | Purpose | Rationale |
|----------|------------|---------|---------|-----------|
| **Programming Language** | {Language} | {Version} | {Primary development language} | {Language choice rationale} |
| **Runtime/Platform** | {Runtime} | {Version} | {Execution environment} | {Platform selection rationale} |
| **Primary Framework** | {Framework} | {Version} | {Application framework} | {Framework selection rationale} |
| **Database** | {Database} | {Version} | {Data persistence} | {Database choice rationale} |
| **Caching** | {Cache solution} | {Version} | {Caching layer} | {Caching strategy rationale} |

### Frontend Technology Stack

{Include this section for projects with user interfaces - remove entirely for backend-only projects}

| Category | Technology | Version | Purpose | Rationale |
|----------|------------|---------|---------|-----------|
| **Frontend Framework** | {Framework} | {Version} | {UI development framework} | {Frontend framework rationale} |
| **UI Library** | {Component library} | {Version} | {Component system} | {UI library choice rationale} |
| **State Management** | {State solution} | {Version} | {Client state management} | {State management rationale} |
| **Build Tool** | {Build system} | {Version} | {Build and bundling} | {Build tool rationale} |
| **Styling** | {CSS approach} | {Version} | {Styling methodology} | {Styling approach rationale} |

### Backend Technology Stack

{Include this section for projects with server-side components - remove entirely for frontend-only projects}

| Category | Technology | Version | Purpose | Rationale |
|----------|------------|---------|---------|-----------|
| **Backend Framework** | {Framework} | {Version} | {Server framework} | {Backend framework rationale} |
| **API Style** | {REST/GraphQL/tRPC} | {Version} | {API communication pattern} | {API approach rationale} |
| **Authentication** | {Auth solution} | {Version} | {Authentication system} | {Auth solution rationale} |
| **File Storage** | {Storage solution} | {Version} | {File and media storage} | {Storage solution rationale} |

### Development and Operations Stack

| Category | Technology | Version | Purpose | Rationale |
|----------|------------|---------|---------|-----------|
| **Testing Framework** | {Test framework} | {Version} | {Testing approach} | {Testing strategy rationale} |
| **CI/CD Platform** | {CI/CD tool} | {Version} | {Continuous integration} | {CI/CD platform rationale} |
| **Infrastructure** | {IaC tool} | {Version} | {Infrastructure as code} | {Infrastructure approach rationale} |
| **Monitoring** | {Monitoring solution} | {Version} | {System monitoring} | {Monitoring strategy rationale} |
| **Deployment** | {Deployment platform} | {Version} | {Application hosting} | {Deployment platform rationale} |

## Data Architecture

{Define the core data structures and their relationships at the conceptual level}

### Data Models

#### {Model Name 1}

**Purpose:** {What this model represents and its role in the system}

**Key Attributes:**
- {attribute_name}: {data_type} - {description and constraints}
- {attribute_name}: {data_type} - {description and constraints}
- {attribute_name}: {data_type} - {description and constraints}

**Relationships:**
- {Relationship description to other models}
- {Relationship description to other models}

#### {Model Name 2}

{Follow the same structure for additional core data entities}

### Database Schema Design

{Include this section for projects requiring data persistence - remove for static sites or external-data-only projects}

**Database Type:** {SQL/NoSQL/Multi-model}

**Schema Approach:** {Normalized/Denormalized/Hybrid}

**Key Schema Decisions:**
- {Schema decision 1: rationale and implications}
- {Schema decision 2: rationale and implications}
- {Schema decision 3: rationale and implications}

### Data Flow Architecture

{Describe how data moves through the system}

```mermaid
graph LR
    A[{Data Source}] --> B[{Validation Layer}]
    B --> C[{Business Logic}]
    C --> D[{Data Storage}]
    D --> E[{API Layer}]
    E --> F[{Client Applications}]
```

{Explain the data flow diagram and transformation points}

## Component Architecture

{Define the major logical components and their responsibilities}

### Component Organization

{Describe how components are organized and interact}

```mermaid
graph TD
    A[{Frontend Components}] --> B[{API Gateway}]
    B --> C[{Business Logic Layer}]
    C --> D[{Data Access Layer}]
    D --> E[{Database}]
    C --> F[{External Services}]
```

### Core Components

#### {Component Name 1}

**Responsibility:** {What this component does and why it exists}

**Key Interfaces:**
- {Interface 1: description of API or contract}
- {Interface 2: description of API or contract}

**Dependencies:**
- {Dependency 1: what it depends on and why}
- {Dependency 2: what it depends on and why}

**Technology Stack:** {Specific technologies used in this component}

#### {Component Name 2}

{Follow the same structure for additional major components}

### Component Communication Patterns

{Describe how components interact with each other}

**Communication Style:** {Synchronous/Asynchronous/Event-driven/Mixed}

**Integration Patterns:** {Description of how components integrate and communicate}

## API Design

{Include this section for projects with API layers - remove for frontend-only projects that don't create APIs}

### API Architecture

**API Style:** {REST/GraphQL/tRPC/Hybrid}

**API Design Principles:**
- {Principle 1: description and application}
- {Principle 2: description and application}
- {Principle 3: description and application}

### API Specification

{Choose the appropriate specification format based on your API style}

#### REST API Specification

{If using REST APIs, provide OpenAPI specification}

```yaml
openapi: 3.0.0
info:
  title: {API Title}
  version: {API Version}
  description: {API Description}
servers:
  - url: {Server URL}
    description: {Server Description}

paths:
  /{endpoint}:
    get:
      summary: {Endpoint description}
      responses:
        '200':
          description: {Success response description}
```

#### GraphQL Schema

{If using GraphQL, provide the schema definition}

```graphql
type {TypeName} {
  {field}: {Type}
  {field}: {Type}
}

type Query {
  {queryName}({parameters}): {ReturnType}
}

type Mutation {
  {mutationName}({parameters}): {ReturnType}
}
```

### Authentication and Authorization

**Authentication Method:** {JWT/OAuth/Session-based/Other}

**Authorization Model:** {Role-based/Attribute-based/Resource-based}

**Security Implementation:** {High-level approach to API security}

## Frontend Architecture

{Include this entire section for projects with user interfaces - remove entirely for backend-only/API-only projects}

### Frontend Framework Configuration

**Framework Choice:** {React/Vue/Angular/Svelte/Other}

**Key Framework Decisions:**
- {Decision 1: rationale and implications}
- {Decision 2: rationale and implications}
- {Decision 3: rationale and implications}

### Project Structure

{Define the directory structure for consistent development}

```
src/
├── components/              # {Reusable UI components}
│   ├── ui/                 # {Basic building blocks}
│   ├── layout/             # {Layout components}
│   └── forms/              # {Form components}
├── pages/                  # {Page-level components}
├── features/               # {Feature-based organization}
│   └── {feature-name}/
│       ├── components/     # {Feature-specific components}
│       ├── hooks/          # {Feature-specific logic}
│       └── services/       # {Feature API services}
├── hooks/                  # {Shared custom hooks}
├── services/               # {API integration layer}
├── stores/                 # {State management}
├── utils/                  # {Utility functions}
├── styles/                 # {Global styles and theme}
├── types/                  # {TypeScript definitions}
└── assets/                 # {Static assets}
```

### State Management Architecture

**State Management Solution:** {Redux/Zustand/Context/Other}

**State Organization:**
- {State slice 1: purpose and scope}
- {State slice 2: purpose and scope}
- {State slice 3: purpose and scope}

**State Management Patterns:**
- {Pattern 1: description and usage}
- {Pattern 2: description and usage}

### Component Standards

**Component Organization:** {How components are structured and organized}

**Naming Conventions:**
- Components: {Naming pattern}
- Files: {File naming pattern}
- Props: {Props naming pattern}

**Component Template:**

```typescript
{import statements}

interface {ComponentName}Props {
  {prop}: {type};
  {prop}: {type};
}

export const {ComponentName}: React.FC<{ComponentName}Props> = ({ {props} }) => {
  {component implementation}

  return (
    {JSX template}
  );
};
```

### Styling Architecture

**Styling Approach:** {CSS Modules/Styled Components/Tailwind/SCSS}

**Design System Integration:** {How styling integrates with design system}

**Responsive Design Strategy:** {Mobile-first/Desktop-first/Component-based}

**Theme Management:** {Approach to theming and design tokens}

## Infrastructure and Deployment

{Define the deployment architecture and infrastructure strategy}

### Deployment Architecture

**Deployment Platform:** {Vercel/Netlify/AWS/Azure/GCP/Other}

**Deployment Strategy:** {Static/Serverless/Container/Traditional}

**Platform Rationale:** {Why this platform was chosen}

### Environment Strategy

{Define different environments and their purposes}

| Environment | Purpose | Configuration | Access |
|-------------|---------|---------------|---------|
| **Development** | {Local development} | {Key config differences} | {Developer access} |
| **Staging** | {Pre-production testing} | {Staging-specific config} | {Team/stakeholder access} |
| **Production** | {Live system} | {Production config} | {Production access controls} |

### Infrastructure as Code

**IaC Approach:** {Terraform/CDK/ARM/Other}

**Infrastructure Components:**
- {Component 1: purpose and configuration}
- {Component 2: purpose and configuration}
- {Component 3: purpose and configuration}

### CI/CD Pipeline

**Pipeline Platform:** {GitHub Actions/GitLab CI/Jenkins/Other}

**Pipeline Stages:**
1. {Stage 1: description and purpose}
2. {Stage 2: description and purpose}
3. {Stage 3: description and purpose}
4. {Stage 4: description and purpose}

**Deployment Process:** {Description of how deployments work}

## Security Architecture

{Define security considerations and implementation approaches}

### Security Strategy

{Describe the overall approach to security in the system}

**Security Principles:**
- {Principle 1: description and implementation}
- {Principle 2: description and implementation}
- {Principle 3: description and implementation}

### Authentication and Authorization

**User Authentication:** {How users authenticate with the system}

**Authorization Model:** {How permissions and access control work}

**Session Management:** {How user sessions are managed}

### Data Protection

**Data Classification:** {How sensitive data is identified and handled}

**Encryption Strategy:** {Encryption requirements for data at rest and in transit}

**Privacy Compliance:** {GDPR/CCPA/other privacy regulation compliance}

### Security Controls

- {Security control 1: description and implementation}
- {Security control 2: description and implementation}
- {Security control 3: description and implementation}

## Testing Strategy

{Define the comprehensive testing approach across the entire system}

### Testing Philosophy

{Describe the overall approach to testing and quality assurance}

### Testing Architecture

**Testing Pyramid:** {Unit/Integration/E2E test distribution}

**Test Organization:** {How tests are structured and organized}

**Test Environment Strategy:** {How test environments are managed}

### Testing Tools and Frameworks

| Test Type | Framework/Tool | Purpose | Coverage |
|-----------|----------------|---------|----------|
| **Unit Tests** | {Testing framework} | {Component/function testing} | {Target coverage} |
| **Integration Tests** | {Testing tool} | {Component integration testing} | {Integration scope} |
| **End-to-End Tests** | {E2E framework} | {User journey testing} | {Critical path coverage} |
| **Performance Tests** | {Performance tool} | {Performance validation} | {Performance targets} |

### Quality Assurance

**Code Quality Tools:** {Linting, formatting, and code analysis tools}

**Code Review Process:** {How code reviews are conducted}

**Quality Gates:** {Quality criteria that must be met before deployment}

## Monitoring and Observability

{Define monitoring, logging, and observability strategy}

### Monitoring Strategy

{Describe the overall approach to system monitoring and observability}

### Application Monitoring

**Monitoring Platform:** {Monitoring solution and rationale}

**Key Metrics:**
- {Metric 1: what it measures and target values}
- {Metric 2: what it measures and target values}
- {Metric 3: what it measures and target values}

**Alerting Strategy:** {When and how alerts are triggered}

### Logging Architecture

**Logging Framework:** {Logging technology and approach}

**Log Aggregation:** {How logs are collected and analyzed}

**Log Retention:** {Log retention policies and storage}

### Performance Monitoring

**Performance Targets:** {Key performance requirements and SLAs}

**Performance Monitoring:** {Tools and techniques for performance tracking}

**Optimization Strategy:** {Approach to performance optimization}

## Project Structure and Development Workflow

{Define the complete project organization and development processes}

### Repository Structure

{Provide the complete project structure}

```
{project-name}/
├── .github/                    # CI/CD workflows and GitHub config
│   └── workflows/
│       ├── ci.yml
│       └── deploy.yml
├── {frontend-directory}/       # Frontend application
│   ├── src/
│   ├── public/
│   ├── tests/
│   └── package.json
├── {backend-directory}/        # Backend application (if applicable)
│   ├── src/
│   ├── tests/
│   └── package.json
├── shared/                     # Shared code and types
│   ├── types/
│   └── utils/
├── infrastructure/             # Infrastructure as code
├── docs/                       # Documentation
├── scripts/                    # Build and deployment scripts
├── .env.example               # Environment template
├── package.json               # Root package.json
└── README.md
```

### Development Workflow

**Local Development Setup:**
1. {Setup step 1}
2. {Setup step 2}
3. {Setup step 3}

**Development Commands:**
- `{command}` - {Purpose}
- `{command}` - {Purpose}
- `{command}` - {Purpose}

**Git Workflow:** {Branching strategy and merge process}

### Environment Configuration

**Required Environment Variables:**

```bash
# Core Configuration
{APP_ENV}={development|staging|production}
{API_BASE_URL}={API base URL}

# Database (if applicable)
{DATABASE_URL}={Database connection string}

# Authentication
{JWT_SECRET}={JWT signing secret}
{AUTH_PROVIDER_CONFIG}={Authentication provider configuration}

# External Services
{EXTERNAL_API_KEY}={External service API key}

# Monitoring
{MONITORING_API_KEY}={Monitoring service API key}
```

**Configuration Management:** {How environment-specific configuration is handled}

## Development Standards

{Establish critical coding standards and development practices}

### Coding Standards

**Universal Standards:**
- {Standard 1: description and enforcement}
- {Standard 2: description and enforcement}
- {Standard 3: description and enforcement}

**Frontend Standards:** {Frontend-specific coding standards}

**Backend Standards:** {Backend-specific coding standards}

### Code Quality Tools

**Linting Configuration:** {ESLint, Prettier, or equivalent configuration}

**Type Checking:** {TypeScript or equivalent type checking requirements}

**Code Formatting:** {Automated formatting standards and tools}

### Documentation Requirements

**Code Documentation:** {Inline documentation requirements}

**API Documentation:** {API documentation standards}

**Architecture Documentation:** {How architecture changes are documented}

## Performance and Scalability

{Define performance requirements and scalability approach}

### Performance Requirements

**Performance Targets:**
- {Metric 1: target value and measurement method}
- {Metric 2: target value and measurement method}
- {Metric 3: target value and measurement method}

**Optimization Strategy:** {Approach to performance optimization}

### Scalability Architecture

**Scaling Strategy:** {Vertical/Horizontal/Auto-scaling approach}

**Bottleneck Analysis:** {Identified potential bottlenecks and mitigation}

**Capacity Planning:** {Growth projections and capacity requirements}

## Risk Assessment and Mitigation

{Identify and address potential architectural risks}

### Technical Risks

**Risk Assessment:**
- {Risk 1: description, probability, impact, mitigation}
- {Risk 2: description, probability, impact, mitigation}
- {Risk 3: description, probability, impact, mitigation}

### Dependencies and Vendor Risk

**External Dependencies:** {Critical external dependencies and alternatives}

**Vendor Lock-in Assessment:** {Vendor lock-in risks and mitigation strategies}

**Technology Risk:** {Technology choice risks and alternatives}

## Next Steps

{Define the immediate actions needed to begin implementation based on this architecture}

### Implementation Phases

**Phase 1:** {Phase description, deliverables, and timeline}

**Phase 2:** {Phase description, deliverables, and timeline}

**Phase 3:** {Phase description, deliverables, and timeline}

### Team Handoff

This Architecture Document provides the complete technical blueprint for {Project Name}. Development teams should use this document as the authoritative source for all technical decisions and implementation approaches.

Key implementation priorities:
1. {Priority 1: description and rationale}
2. {Priority 2: description and rationale}
3. {Priority 3: description and rationale}

### Architecture Validation

**Review Requirements:** {What architectural reviews are needed}

**Validation Criteria:** {How to validate that implementation follows architecture}

**Change Management:** {How architectural changes will be managed and documented}

---
