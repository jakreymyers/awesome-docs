# Writing Guide: Architecture

>Before using [Template: Architecture Greenfield](./template_architecture-greenfield.md) or [Template: Architecture Brownfield](./template_architecture-brownfield.md), read this for guidance on template selection and how to fill in these templates.

## Why do I need an architecture document?

Architecture documents serve as the technical foundation that bridges the gap between product requirements and actual implementation. They provide the authoritative blueprint that guides development teams through complex technical decisions while ensuring consistency across the entire system.

For AI-driven development workflows, a well-structured architecture document becomes the primary technical reference that enables autonomous development agents to make informed implementation choices. It reduces ambiguity, prevents architectural drift, and ensures that all technical decisions align with project goals and constraints.

As projects evolve from initial design through production deployment, the architecture document serves as both a decision-making framework and a validation checkpoint, ensuring that implementation stays true to architectural principles while accommodating necessary changes through structured change management.

## Template Selection Guide

The choice between greenfield and brownfield architecture templates depends fundamentally on your project's relationship with existing systems. This decision affects every aspect of your architectural planning, from technology selection to integration complexity.

### Understanding the Templates

**Architecture Greenfield** is designed for projects where you have complete technical freedom to choose optimal solutions. You're starting fresh, which means you can select the best technology stack, design ideal system patterns, and optimize for future requirements without worrying about legacy constraints or existing system compatibility.

**Architecture Brownfield** addresses the complexities of working within existing system constraints. These projects require careful analysis of current architecture, detailed compatibility planning, and sophisticated integration strategies to ensure new components work seamlessly with established systems.

### Quick Selection Guide

| Project Context | Template Choice | Key Considerations |
|-----------------|-----------------|-------------------|
| Building new systems from scratch | Architecture Greenfield | Complete technology freedom |
| Enhancing existing applications | Architecture Brownfield | Integration and compatibility focus |
| Rebuilding legacy systems completely | Architecture Greenfield | Clean slate approach |
| Adding features to current systems | Architecture Brownfield | Constraint-driven design |

### When to Choose Architecture Greenfield

Choose the greenfield template when you're designing completely new systems where technical decisions can be optimized for current requirements rather than constrained by existing choices. This includes startup projects, proof-of-concepts, complete system rebuilds, or new products that don't need to integrate with established infrastructure.

The key indicator for greenfield projects is freedom of choice. If you can select any database, any framework, any hosting platform based purely on what's best for your requirements, you're in greenfield territory. For example, designing a new microservices architecture with modern containerization represents a classic greenfield scenario.

Greenfield projects benefit from this template's comprehensive coverage of technology selection rationale, optimal architectural patterns, and forward-looking scalability planning. The template guides you through making foundational decisions that will serve the project throughout its lifecycle.

### When to Choose Architecture Brownfield

The brownfield template becomes essential when your architectural decisions must work within existing system constraints. This applies to feature additions, system enhancements, modernization projects, or any development where you must preserve current functionality while adding new capabilities.

Consider brownfield when you find yourself asking: "How will this affect existing users?" or "What happens to current data?" These questions indicate the need for integration analysis and compatibility planning that the brownfield template specifically addresses.

For instance, modernizing the user interface of an established enterprise application requires understanding current data flows, API contracts, and user workflows—exactly the type of analysis the brownfield template guides you through.

### Architecture Scope Considerations

Architecture documents can serve different scopes depending on your project needs. Consider whether you're documenting:

- **Full-stack architecture** covering both frontend and backend systems
- **Backend-only architecture** for API services or data processing systems
- **Frontend-only architecture** for user interface applications
- **System integration architecture** focusing on how multiple systems connect

Both templates are designed with modular sections that can be included or removed based on your scope. A backend-only project can simply remove the frontend sections, while a frontend-only project can focus on component architecture and user experience patterns.

## Architecture Best Practices

### Comprehensive Yet Focused

Effective architecture documents balance comprehensive coverage with practical focus. They should address all major technical decisions without getting lost in implementation details that belong in detailed design documents.

Start with high-level architectural patterns and work down to component-level decisions. Each level should provide enough detail for the next level of planning while remaining technology-agnostic enough to allow implementation flexibility.

Architecture documents serve multiple audiences—from business stakeholders who need to understand technical approach to developers who need specific guidance. Structure your content to serve both audiences effectively.

### Technology Selection and Rationale

Every technology choice in your architecture should include clear rationale that can be evaluated and questioned. Rather than simply stating "we'll use React," explain why React serves your requirements better than alternatives.

Technology rationale becomes particularly important for long-lived projects where original decision-makers may not be available to explain choices. Future maintainers need to understand not just what technologies are used, but why they were chosen and under what constraints.

For brownfield projects, technology choices must also consider integration requirements and migration complexity. The best technology in isolation may not be the best choice when integration costs are considered.

### Scalability and Future Planning

Architecture documents should address both current requirements and reasonable future growth. This doesn't mean over-engineering for hypothetical scale, but rather making informed decisions about where flexibility is worth the investment.

Consider scalability at multiple levels: user growth, data volume, feature complexity, and team size. Each type of growth creates different architectural pressures that should be anticipated in your design decisions.

Document specific scaling strategies and trigger points where architectural changes would be needed. This helps teams plan for growth rather than react to scaling crises.

## Template Structure and Customization

### Modular Section Organization

Both architecture templates are organized with modular sections that can be included or removed based on your project scope. This allows a single template to serve frontend-only, backend-only, or full-stack projects.

**Core Sections** (always needed):
- Introduction and project context
- High-level architecture overview
- Technology stack decisions
- Development workflow and standards

**Frontend Sections** (remove for backend-only projects):
- Frontend architecture and component design
- State management and UI patterns
- User experience considerations
- Client-side performance optimization

**Backend Sections** (remove for frontend-only projects):
- API design and data architecture
- Database schema and data flow
- Server-side scalability patterns
- Infrastructure and deployment strategy

**Shared Sections** (usually applicable):
- Security architecture and implementation
- Testing strategy across the stack
- Monitoring and observability approach
- Risk assessment and mitigation

### Section-by-Section Guidance

### High Level Architecture

This section establishes the foundational understanding that guides all subsequent technical decisions. Think of it as your project's technical north star—every implementation choice should trace back to these core architectural principles.

Start with a clear technical summary that explains your overall approach in terms that both technical and business stakeholders can understand. Avoid jargon while still providing enough technical detail to guide implementation decisions.

The architectural pattern choice (monolithic, microservices, serverless, etc.) fundamentally affects every other technical decision. Document not just what pattern you've chosen, but why it fits your specific requirements, team capabilities, and operational constraints.

For greenfield projects, focus on optimal patterns that serve your requirements and growth projections. Consider team expertise, operational complexity, and long-term maintenance when selecting patterns.

Brownfield projects must balance optimal architecture with integration reality. Sometimes the best architectural pattern is the one that works well with existing systems, even if it wouldn't be your first choice for a greenfield project.

### Technology Stack Decisions

Your technology stack table should serve as the definitive reference for all technology choices throughout the project. Each technology entry needs clear rationale that future team members can understand and evaluate.

Strong technology rationale addresses multiple factors: technical capabilities, team expertise, ecosystem maturity, community support, and long-term viability. The goal is enabling informed decisions, not defending arbitrary choices.

Consider the interaction between technologies in your stack. The best individual choices don't always create the best integrated system. Document how your chosen technologies work together and what integration challenges you've considered.

For brownfield projects, technology choices must also address migration complexity and compatibility requirements. Sometimes maintaining consistency with existing technologies outweighs the benefits of newer alternatives.

Version specifications matter more than many teams realize. Document specific versions and any known compatibility constraints. This prevents subtle bugs and deployment issues that arise from version mismatches.

### Data Architecture and Schema Design

Data architecture decisions have long-lasting implications that are expensive to change later. Approach data modeling with careful consideration of both current requirements and reasonable future evolution.

Start with conceptual data models that focus on relationships and business logic rather than implementation details. These models should be understandable by both technical teams and business stakeholders who need to validate that the architecture serves business needs.

Database technology choices should align with your data access patterns, consistency requirements, and scalability projections. Document the trade-offs you've considered—consistency vs. availability, SQL vs. NoSQL, single database vs. polyglot persistence.

For brownfield projects, data architecture becomes particularly complex because you must consider migration strategies, backward compatibility, and integration with existing data stores. Document how new data structures will coexist with existing ones and what migration approach you'll use.

Performance implications of data architecture decisions should be explicitly considered. How will your schema design perform under expected load? What indexing strategies will be needed? Where are the likely bottlenecks?

### Component Architecture and Organization

Component architecture defines how your system is organized and how different parts interact. Good component design makes systems easier to understand, test, and maintain while enabling team scalability.

For frontend applications, component architecture involves both technical organization (how components are structured in code) and logical organization (how components relate to user workflows and business functionality).

Backend component architecture focuses on service boundaries, data flow, and integration patterns. Whether you're building a monolith or microservices, clear component boundaries help teams work independently while maintaining system coherence.

Component communication patterns deserve special attention. How do components share data? How do they handle errors? How do they coordinate complex workflows? These patterns should be consistent across your system.

Dependency management becomes crucial as systems grow. Document how components depend on each other and what strategies you'll use to minimize coupling while enabling necessary coordination.

### API Design and Integration

API design serves as the contract between different parts of your system and external consumers. Well-designed APIs enable flexibility and evolution while poorly designed APIs create technical debt that's expensive to fix.

Choose your API style (REST, GraphQL, tRPC) based on your specific use cases rather than industry trends. Each style has strengths and weaknesses that should align with your requirements for flexibility, performance, and development velocity.

API documentation should be comprehensive enough that consumers can integrate successfully without additional consultation. This includes not just endpoint specifications, but also authentication, error handling, rate limiting, and versioning strategies.

For brownfield projects, API evolution strategy becomes critical. How will you add new capabilities while maintaining backward compatibility? What versioning approach will you use? How will you communicate changes to existing consumers?

Security considerations should be built into API design from the beginning rather than added later. Authentication, authorization, input validation, and rate limiting should all be considered as part of your core API architecture.

### Infrastructure and Deployment Architecture

Infrastructure decisions affect every aspect of your system's operation, from development workflow to production scalability. Consider infrastructure as part of your architecture rather than an afterthought.

Cloud platform choice should align with your technical requirements, team expertise, and cost constraints. Each platform has strengths that may align better with your specific needs—avoid choosing based on familiarity alone.

Deployment strategy affects both development velocity and operational reliability. Consider how your deployment approach supports testing, rollback, monitoring, and scaling requirements.

Environment strategy should support your development workflow while providing appropriate isolation and security. Consider how many environments you need, how they differ, and how changes flow between them.

Infrastructure as code becomes essential for any system that will be maintained over time. Document your IaC approach and how infrastructure changes will be managed and deployed.

### Security Architecture Integration

Security should be integrated into your architecture from the beginning rather than added as an afterthought. Consider security at every level from data storage to user interface design.

Authentication and authorization patterns should be consistent across your system while being appropriate for your specific requirements. Consider both current needs and likely future requirements when designing these systems.

Data protection requirements vary significantly based on your application domain and regulatory environment. Document your data classification approach and how different types of data will be protected throughout their lifecycle.

For brownfield projects, security integration must consider existing security measures and compliance requirements. How will new functionality integrate with existing authentication systems? What additional security measures are needed?

Threat modeling should inform your security architecture decisions. What are the most likely attack vectors? How will your architecture detect and respond to security incidents? What data would be most valuable to attackers?

### Testing Strategy Architecture

Testing strategy should be considered as part of your architecture because it affects system design decisions. Systems that are designed for testability are generally better architected overall.

The testing pyramid concept helps balance comprehensive coverage with maintainable test suites. Consider how your architecture supports unit testing, integration testing, and end-to-end testing at each level.

Test environment strategy should align with your architecture complexity. How will you test complex integrations? How will you handle test data management? How will you isolate tests from each other?

For brownfield projects, testing strategy must address both new functionality and regression testing for existing capabilities. How will you ensure that enhancements don't break existing functionality?

Automated testing should be integrated into your development workflow from the beginning. Consider how your architecture supports continuous integration, automated deployment, and production monitoring.

## Template Customization Matrix

### Frontend-Only Projects

For projects focused entirely on user interface development, you can streamline the architecture template by removing backend-specific sections while enhancing frontend coverage.

**Include These Sections:**
- High Level Architecture (focus on frontend patterns)
- Frontend Technology Stack
- Component Architecture and Organization
- State Management Architecture
- API Integration (consuming external APIs)
- User Experience and Design System Integration
- Frontend Performance and Optimization
- Browser Compatibility and Accessibility
- Testing Strategy (frontend-focused)
- Deployment and Hosting (static sites/SPAs)

**Remove These Sections:**
- Backend Technology Stack
- Database Schema Design
- API Design and Implementation
- Server-Side Infrastructure
- Backend Security Implementation

**Adapt These Sections:**
- Security (focus on client-side security, authentication integration)
- Monitoring (focus on client-side monitoring, error tracking)
- Performance (focus on loading, rendering, user experience metrics)

### Backend-Only Projects

For API services, data processing systems, or server-side applications without user interfaces, focus on server-side architecture while removing frontend considerations.

**Include These Sections:**
- High Level Architecture (focus on service patterns)
- Backend Technology Stack
- Data Architecture and Database Design
- API Design and Implementation
- Component Architecture (service boundaries)
- Infrastructure and Deployment
- Security Architecture
- Database Performance and Optimization
- Testing Strategy (API and service testing)
- Monitoring and Observability

**Remove These Sections:**
- Frontend Technology Stack
- Component Architecture (UI components)
- State Management (client-side)
- User Experience Design
- Browser Compatibility

**Adapt These Sections:**
- Performance (focus on API response times, throughput, scalability)
- Testing (focus on API testing, service integration testing)
- Deployment (focus on service deployment, database migrations)

### Full-Stack Projects

Full-stack projects benefit from the complete template but should pay special attention to integration points between frontend and backend systems.

**Emphasize These Areas:**
- API design as the contract between frontend and backend
- Data flow from database through API to user interface
- Authentication and authorization across the entire stack
- Error handling and user feedback loops
- End-to-end testing strategies
- Deployment coordination between frontend and backend
- Monitoring across all system layers

**Integration Considerations:**
- How frontend state management aligns with backend data models
- How API design supports frontend user experience requirements
- How security measures coordinate across the entire system
- How performance optimization works across all layers

## Decision Trees and Selection Criteria

### Architecture Pattern Selection

```
What is your primary scalability requirement?
├─ Team scalability (multiple teams, independent development)
│  ├─ High → Consider microservices or service-oriented architecture
│  └─ Medium → Consider modular monolith with clear service boundaries
└─ Technical scalability (traffic, data volume)
   ├─ Extreme → Consider microservices with event-driven patterns
   ├─ High → Consider service-oriented architecture or microservices
   └─ Medium → Consider monolithic architecture with horizontal scaling
```

### Technology Stack Selection

```
What is your team's primary constraint?
├─ Timeline pressure
│  ├─ Use familiar technologies with proven integration patterns
│  └─ Prioritize rapid prototyping and iteration capabilities
├─ Technical requirements
│  ├─ Performance critical → Choose technologies optimized for your use case
│  └─ Scalability critical → Choose technologies with proven scaling patterns
└─ Team expertise
   ├─ Strong in specific stack → Leverage existing expertise
   └─ Learning opportunity → Balance learning with delivery requirements
```

### Deployment Strategy Selection

```
What is your operational complexity tolerance?
├─ Minimal operational overhead
│  ├─ Choose managed platforms (Vercel, Netlify, Heroku)
│  └─ Prioritize simplicity over customization
├─ Moderate operational complexity
│  ├─ Choose cloud platforms with good abstractions (AWS ECS, Google Cloud Run)
│  └─ Balance control with operational burden
└─ High operational complexity acceptable
   ├─ Choose infrastructure-as-code with full control (Kubernetes, custom infrastructure)
   └─ Optimize for specific requirements over operational simplicity
```

## Common Architecture Pitfalls and Solutions

### Over-Engineering for Unknown Future Requirements

Many architecture documents suffer from premature optimization for theoretical future needs that may never materialize. This leads to unnecessary complexity that slows current development without providing real benefits.

The solution is focusing on current requirements while building in specific flexibility for likely future changes. Document what assumptions you're making about future growth and what indicators would trigger architectural changes.

Instead of building for unlimited scale from day one, design systems that can evolve toward higher scale when specific thresholds are reached. This approach balances future planning with practical development velocity.

### Under-Specifying Technology Integration

Architecture documents sometimes specify individual technologies without addressing how they work together. This leads to integration problems during implementation that could have been avoided with better planning.

Effective architecture documents address technology integration explicitly. How does your frontend framework work with your API design? How does your database choice align with your scaling strategy? How do your monitoring tools integrate with your deployment platform?

Consider creating integration diagrams that show how different technologies in your stack communicate and depend on each other. This helps identify potential integration issues before implementation begins.

### Ignoring Team and Organizational Constraints

Technical architecture must align with team capabilities and organizational constraints. The most elegant technical solution may not be the best choice if your team lacks the expertise to implement and maintain it effectively.

Consider team size, expertise, and growth plans when making architectural decisions. A small team might benefit from simpler architectures even if more complex patterns would theoretically be superior.

Document the team and organizational assumptions underlying your architectural choices. This helps future decision-makers understand when architectural changes might be needed as the organization evolves.

### Inadequate Error Handling and Monitoring Strategy

Many architecture documents focus on happy-path scenarios while under-specifying error handling, monitoring, and debugging strategies. This leads to systems that are difficult to operate and debug in production.

Effective architecture documents address observability as a first-class concern. How will you detect when things go wrong? How will you debug complex issues that span multiple components? How will you measure system health and performance?

Consider error handling patterns that are consistent across your system while being appropriate for different types of failures. Network errors, validation errors, and system failures may require different handling strategies.

### Brownfield Integration Underestimation

Brownfield projects often underestimate the complexity of integrating with existing systems. Architecture documents may focus on new functionality while inadequately addressing compatibility and migration requirements.

Successful brownfield architecture requires thorough analysis of existing systems and careful planning of integration strategies. Document what you know about existing systems, what assumptions you're making, and what risks you've identified.

Consider creating separate sections for integration architecture that address how new and existing systems will work together during both implementation and long-term operation.

### Security as an Afterthought

Security considerations are often deferred to implementation phases rather than being integrated into architectural planning. This leads to security measures that feel bolted-on rather than integrated into the system design.

Effective security architecture integrates security considerations into every architectural decision. How does your component design support security boundaries? How does your API design prevent common vulnerabilities? How does your data architecture protect sensitive information?

Consider threat modeling as part of your architectural process. What are the most likely attack vectors for your system? How will your architecture detect and respond to security incidents?

## Quality Assurance and Validation

### Architecture Document Completeness

Before finalizing your architecture document, verify that it addresses all major technical decisions and provides sufficient guidance for implementation teams.

**Technical Completeness Checklist:**
- [ ] All major technology choices are documented with rationale
- [ ] Component boundaries and interactions are clearly defined
- [ ] Data flow and storage strategies are specified
- [ ] Security and authentication approaches are documented
- [ ] Testing and quality assurance strategies are defined
- [ ] Deployment and operational considerations are addressed
- [ ] Performance and scalability requirements are planned for
- [ ] Risk assessment and mitigation strategies are included

**Audience Appropriateness Checklist:**
- [ ] Technical stakeholders have sufficient detail for implementation planning
- [ ] Business stakeholders can understand technical approach and implications
- [ ] Future maintainers have enough context to understand architectural decisions
- [ ] Integration teams have clear specifications for system boundaries

### Stakeholder Review and Validation

Architecture documents should be reviewed by multiple stakeholders to ensure technical feasibility, business alignment, and operational viability.

**Technical Review Focus Areas:**
- Technology integration feasibility and complexity
- Performance and scalability assumptions and plans
- Security and compliance requirement coverage
- Testing and quality assurance adequacy
- Operational and maintenance consideration completeness

**Business Review Focus Areas:**
- Alignment with business requirements and constraints
- Timeline and resource requirement reasonableness
- Risk assessment and mitigation strategy adequacy
- Long-term maintenance and evolution planning

**Operational Review Focus Areas:**
- Deployment and infrastructure requirement feasibility
- Monitoring and debugging capability adequacy
- Security and compliance control implementation
- Team capability and training requirement assessment

### Architecture Evolution Planning

Document how your architecture will evolve over time and what triggers would indicate the need for architectural changes.

**Evolution Indicators:**
- Performance or scalability limits being approached
- Team size or structure changes requiring different patterns
- Business requirement changes affecting fundamental assumptions
- Technology ecosystem changes creating new opportunities or requirements

**Change Management Process:**
- How architectural changes will be proposed and evaluated
- What approval processes are needed for different types of changes
- How changes will be documented and communicated
- How implementation teams will be guided through architectural transitions

---

This guide provides comprehensive direction for creating effective architecture documents that serve as authoritative technical blueprints for AI-powered development workflows. Choose the appropriate template based on your project context, and use this guidance to ensure your architecture document provides clear technical direction while remaining flexible enough to evolve with your project's needs.
