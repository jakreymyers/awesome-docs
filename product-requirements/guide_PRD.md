# Writing Guide: Product Requirements Document (PRD)

>Before using [Template: PRD Greenfield](./template_PRD-greenfield.md) or [Template: PRD Brownfield](./template_PRD-brownfield.md), read this for guidance on template selection and how to fill in these templates.

## Why do I need a PRD?

A Product Requirements Document (PRD) serves as the foundational blueprint that transforms project ideas into actionable development plans. A PRD defines what will be built, why it should be built, and the specific criteria for success.

The PRD bridges the gap between business vision and technical implementation, ensuring all stakeholders have a shared understanding of project goals, requirements, and deliverables. For AI-driven development workflows, a well-structured PRD becomes the primary source of truth that guides autonomous development agents through complex multi-epic implementations.

As projects evolve from initial concept to production deployment, the PRD serves as both a planning document and a validation checklist, ensuring that development stays aligned with original objectives while accommodating necessary changes through structured change management.

## Template Selection Guide

The choice between greenfield and brownfield PRD templates depends fundamentally on whether you're starting fresh or working with existing systems. This decision shapes every aspect of your requirements gathering and development approach.

### Understanding the Templates

**PRD Greenfield** is designed for new projects where you have complete creative and technical freedom. You're starting with a blank slate, which means you can choose the optimal technology stack, design ideal user workflows, and architect systems for future growth without worrying about legacy constraints.

**PRD Brownfield** addresses the complexities of enhancing existing systems. These projects require careful analysis of current architecture, compatibility planning, and risk mitigation strategies to ensure new features integrate seamlessly without disrupting existing functionality.

### Quick Selection Guide

| Project Situation | Template Choice | Why This Works |
|-------------------|-----------------|----------------|
| Building something completely new | PRD Greenfield | Freedom to optimize everything |
| Adding to existing systems | PRD Brownfield | Handles integration complexity |
| New project using external APIs | PRD Greenfield | Focus on your system design |
| Modernizing legacy applications | PRD Brownfield | Manages migration risks |

### When to Choose PRD Greenfield

Choose the greenfield template when you're creating something new from the ground up. This includes startup products, proof-of-concepts, or when your organization decides to completely rebuild rather than enhance existing systems.

A good indicator is asking yourself: "Can I make any technology choice I want?" If the answer is yes, you're likely in greenfield territory. For example, building a new customer portal with modern React and cloud infrastructure represents a classic greenfield scenario.

### When to Choose PRD Brownfield

The brownfield template becomes essential when you're working within the constraints of existing systems. This applies to feature additions, system integrations, or any enhancement where you must preserve current functionality.

Consider the brownfield approach when you find yourself asking: "How will this affect our current users?" or "What happens to existing data?" These questions signal the need for compatibility analysis and integration planning that the brownfield template provides.

For instance, adding real-time notifications to an established e-commerce platform requires understanding current user workflows, database schemas, and API contracts—exactly what the brownfield template addresses.

### Making the Decision

Still uncertain? Consider your constraints rather than your goals. Greenfield projects are defined by their freedom to choose optimal solutions. Brownfield projects are defined by their need to work within existing constraints while delivering value.

Most organizations lean toward brownfield scenarios more often than they initially realize, simply because truly independent new projects are relatively rare in established companies.

## PRD Best Practices

### Scope and Focus
- **Single Product Focus**: Dedicate each PRD to one cohesive product or major feature set
- **Epic-Driven Organization**: Structure requirements around deployable, value-delivering epics
- **Measurable Criteria**: Every requirement should be testable and verifiable
- **Stakeholder Alignment**: Write for both technical teams and business stakeholders

### Requirements Quality
- **User-Centric Language**: Frame requirements from user perspective and business value
- **Specific and Actionable**: Avoid vague requirements that lead to implementation ambiguity
- **Traceable Dependencies**: Clear relationships between requirements and epics
- **Acceptance Criteria**: Define "done" criteria for every story and epic

### Technical Integration
- **Architecture Alignment**: Ensure technical assumptions align with actual project capabilities
- **Technology Constraints**: Document platform, framework, and integration limitations
- **Testing Strategy**: Define comprehensive testing approach for quality assurance
- **Deployment Readiness**: Include deployment and operational considerations

## Template Structure Comparison

| Section | Greenfield | Brownfield | Purpose |
|---------|------------|------------|---------|
| **Goals & Background** | ✓ Standard | ✓ Enhanced | Project foundation and rationale |
| **Project Analysis** | ✗ Not needed | ✓ Critical | Existing system assessment |
| **Requirements** | ✓ Functional/Non-functional | ✓ + Compatibility | System capabilities definition |
| **UI Design Goals** | ✓ Full design freedom | ✓ Integration-focused | User experience planning |
| **Technical Assumptions** | ✓ Technology selection | ✓ Integration constraints | Architecture foundation |
| **Epic Structure** | ✓ Feature-driven | ✓ + Integration verification | Development organization |
| **Next Steps** | ✓ Team handoffs | ✓ + Risk mitigation | Implementation preparation |

## Section-by-Section Guidance

### Goals and Background Context

This section establishes the foundational understanding that drives all subsequent requirements and technical decisions. Think of it as your project's north star—everything else should trace back to these core goals and the context that justifies them.

#### Writing Effective Goals

Strong PRD goals are specific, measurable, and tied to business value. Rather than saying "improve user experience," specify how you'll measure improvement and what business outcome it drives. Goals should answer what success looks like from both a user and business perspective.

For greenfield projects, focus on market opportunity and the value proposition of your new solution. Why does this product need to exist? What gap are you filling? Greenfield goals often center on capturing market share, addressing unmet user needs, or creating new value propositions.

Consider this greenfield example: A project management tool might aim to "capture 15% market share in the small business project management space within 18 months by focusing on simplified collaboration features." This goal is specific, measurable, and tied to market opportunity.

Brownfield projects require different goal framing. Here you're enhancing existing systems, so goals typically focus on improving current metrics, addressing known pain points, or expanding capabilities. Always reference existing performance metrics and user feedback to justify enhancement needs.

A brownfield goal might read: "Reduce checkout abandonment from 34% to under 20% within 6 months by modernizing the checkout flow based on mobile usability research." This directly addresses a measured problem with a specific improvement target.

#### Crafting Compelling Background

Your background section should tell the story of why this project matters now. For greenfield projects, this might involve market research, competitive analysis, or user research that validates demand for your solution.

For brownfield projects, focus on the gap between current state and desired state. What specific problems does the existing system have? How do you know these are problems worth solving? User analytics, support ticket themes, and competitive pressure all provide compelling background context.

The most effective background sections combine quantitative data with qualitative insights. Numbers prove the problem exists; user stories explain why it matters to real people.

#### Common Mistakes to Avoid

Don't confuse goals with features. "Add a dashboard" is a feature; "increase user engagement by 25% through improved data visibility" is a goal that might be achieved with a dashboard.

Avoid vague metrics like "improve user experience" or "increase performance." These can't be measured or validated. Every goal should have clear success criteria.

For brownfield projects, don't assume readers understand the current system's problems. Provide enough context about existing limitations without diving into technical implementation details.

### Requirements Definition

Requirements form the core contract between stakeholders and development teams. They define what the system must do (functional requirements) and how well it must do it (non-functional requirements). Well-written requirements prevent scope creep, reduce development risk, and provide clear success criteria.

#### Writing Functional Requirements

Functional requirements describe specific capabilities users need from the system. The best functional requirements start with clear action verbs and specify measurable outcomes. Instead of "users can search," write "users can search product catalog by name, category, or price range with results returned in under 2 seconds."

Each requirement should align with complete user workflows rather than isolated features. Think about the entire user journey from goal to completion. For example, a search requirement should consider not just finding items, but also handling no results, filtering large result sets, and saving search criteria.

Don't forget edge cases and error scenarios. What happens when search returns no results? How does the system handle malformed queries? These scenarios often reveal missing requirements that become expensive to address later in development.

For brownfield projects, functional requirements must consider existing system behavior. Users have learned current workflows, and dramatic changes can harm usability even when new features are technically superior. Document which existing behaviors must be preserved and which can be enhanced.

#### Defining Non-Functional Requirements

Non-functional requirements define quality attributes—how the system performs, not what it does. Performance requirements should specify concrete metrics: "API responses complete within 200ms for 95% of requests under normal load" rather than "the system should be fast."

Security requirements are particularly critical for brownfield projects where new features must integrate with existing authentication and authorization systems. Be specific about data classification, encryption requirements, and compliance standards.

Scalability requirements should reflect realistic growth projections based on business goals. If your PRD targets 10,000 new users within 12 months, your scalability requirements should support that growth plus reasonable buffer.

Usability requirements often get overlooked but are essential for user adoption. Consider accessibility standards (WCAG AA compliance), mobile responsiveness, and browser support. For brownfield projects, maintaining consistency with existing interface patterns may be more important than implementing the latest design trends.

#### Brownfield Compatibility Considerations

Brownfield projects face unique compatibility challenges that greenfield projects avoid. API compatibility becomes critical when other systems depend on existing endpoints. You may need versioning strategies or gradual migration approaches to introduce breaking changes safely.

Data migration requirements deserve special attention. How will existing data map to new schemas? What happens to historical data? Can migration happen gradually or does it require downtime? These questions often reveal complex requirements that significantly impact project scope.

User workflow compatibility can be tricky to balance. You want to improve the user experience without forcing users to relearn familiar processes. Consider progressive enhancement approaches that introduce new capabilities while preserving familiar workflows.

### User Interface Design Goals

#### Overall UX Vision
Define the intended user experience philosophy that guides all design decisions. Consider how the interface should feel to users and what interaction paradigms best serve user goals.

#### For Greenfield Projects
- Freedom to define optimal user experience without constraints
- Opportunity to implement modern interaction patterns and accessibility standards
- Focus on user workflow optimization and conversion funnel design

#### For Brownfield Projects
- **Consistency Requirements**: Visual and interaction alignment with existing interface patterns
- **Component Integration**: Reuse of existing design system components and patterns
- **Navigation Harmony**: New features must integrate seamlessly with existing navigation
- **User Training**: Minimize learning curve by leveraging familiar interaction patterns

### Technical Assumptions and Constraints

#### Architecture Decisions
Document high-level architectural patterns that influence all development decisions:
- **Service Architecture**: Monolith, microservices, serverless, or hybrid approaches
- **Repository Structure**: Monorepo vs. polyrepo organization strategy
- **Testing Strategy**: Unit, integration, and end-to-end testing requirements

#### For Greenfield Projects
Focus on technology selection rationale and architectural patterns that optimize for project goals, team expertise, and scalability requirements.

#### For Brownfield Projects
- **Existing Technology Stack**: Document current technologies with version constraints
- **Integration Strategy**: How new components integrate with existing architecture
- **Migration Path**: Approach for transitioning between old and new functionality
- **Risk Mitigation**: Strategies for minimizing impact on existing system stability

### Epic and Story Organization

#### Epic Structure Principles
- **Value Delivery**: Each epic must deliver end-user value and be independently deployable
- **Logical Sequence**: Epics should build progressively toward complete product functionality
- **Risk Management**: Earlier epics should validate core assumptions and reduce project risk
- **Size Optimization**: Epics sized for 2-4 week development cycles with multiple stories

#### Story Writing Standards
- **User-Centric Format**: "As a [user type], I want [capability], so that [benefit]"
- **Acceptance Criteria**: 3-5 specific, testable criteria that define completion
- **Vertical Slices**: Stories should deliver complete functionality across the full stack
- **AI Agent Sizing**: Stories should be completable in 2-4 hours of focused development

#### For Brownfield: Integration Verification
Add integration verification criteria to each story:
- **Existing Functionality**: Verification that current features remain intact
- **Performance Impact**: Confirmation that changes don't degrade system performance
- **Compatibility**: Testing that integrations work correctly with existing systems

## Advanced PRD Techniques

### Change Management
- **Version Control**: Track all PRD changes with dates, descriptions, and rationale
- **Stakeholder Communication**: Notify affected teams of requirement changes
- **Impact Assessment**: Evaluate how changes affect development timeline and scope
- **Approval Process**: Define who must approve significant requirement changes

### Requirements Traceability
- **Epic Mapping**: Clear connections between requirements and epic structure
- **Story Validation**: Each story should trace back to specific functional requirements
- **Testing Alignment**: Requirements should map to specific test cases and validation criteria
- **Feature Completeness**: Ensure all requirements are addressed by at least one epic

### Stakeholder Engagement
- **Review Cycles**: Schedule regular PRD reviews with business and technical stakeholders
- **Feedback Integration**: Process for incorporating stakeholder input into requirements
- **Assumption Validation**: Regular validation of technical and business assumptions
- **Risk Communication**: Transparent communication of project risks and mitigation strategies

## Quality Assurance Checklist

### Requirements Completeness
- [ ] All functional requirements have acceptance criteria
- [ ] Non-functional requirements include measurable criteria
- [ ] UI requirements address all target platforms and devices
- [ ] Technical assumptions are validated and documented

### Epic and Story Validation
- [ ] Every requirement is addressed by at least one epic
- [ ] Stories follow proper user story format with acceptance criteria
- [ ] Epic sequence delivers value incrementally
- [ ] Story sizing appropriate for AI agent execution (2-4 hours)

### Template-Specific Validation

#### For Greenfield PRDs
- [ ] Technology stack selection is justified and appropriate
- [ ] Architecture decisions align with project goals and team capabilities
- [ ] No assumptions about existing systems or legacy constraints

#### For Brownfield PRDs
- [ ] Existing project analysis is thorough and accurate
- [ ] Compatibility requirements address all integration points
- [ ] Risk assessment covers impact on existing functionality
- [ ] Integration verification criteria included in all stories

### Handoff Readiness
- [ ] UX team has sufficient design direction from UI requirements
- [ ] Architecture team has clear technical constraints and assumptions
- [ ] Development team has actionable epics with prioritized story backlog
- [ ] All stakeholders have reviewed and approved the PRD

## Common PRD Pitfalls and Solutions

Even experienced teams fall into predictable traps when writing PRDs. Understanding these common pitfalls can help you avoid costly mistakes and rework.

### Over-Engineering Requirements

One of the most frequent mistakes is confusing requirements with implementation details. Requirements should specify what the system needs to accomplish, not how it accomplishes those goals. When you write "the system must use PostgreSQL database," you're making implementation decisions that belong in architecture documents.

This becomes particularly problematic when technical assumptions conflict with business requirements. You might specify a particular database technology without knowing if it can actually meet your performance requirements or if your team has the expertise to implement it effectively.

The solution is maintaining clear separation between "what" and "how." Instead of "the system must use PostgreSQL database with Redis caching," write "the system must support 10,000 concurrent users with sub-2-second response times." This gives architects freedom to choose the best implementation while ensuring business needs are met.

### Scope Creep Through Requirements Expansion

Scope creep often disguises itself as harmless requirement additions. Stakeholders request "small additions" that seem reasonable in isolation but collectively transform project scope. Each new requirement interacts with existing ones, creating complexity that's difficult to predict.

Watch for warning signs like requirements lists that grow beyond initial estimates or epic structures that become unbalanced as new functionality gets squeezed in. The real danger is when these additions happen without corresponding adjustments to timeline or resources.

Effective change management requires impact assessment for every requirement change, no matter how small it seems. What other requirements does this change affect? How does it impact the epic structure? What's the estimated development cost? These questions help stakeholders make informed decisions about scope changes.

### Vague Acceptance Criteria

Acceptance criteria that use subjective terms like "user-friendly" or "fast" create problems during development and testing. These criteria can't be objectively verified, leading to disagreements about when stories are actually complete.

The most problematic vague criteria are those that sound specific but aren't measurable. "The application should load quickly" seems clear until you ask: quickly compared to what? On which devices? Under what conditions?

Effective acceptance criteria specify measurable outcomes that can be verified through testing or demonstration. "User can reach any main feature within 3 clicks from the dashboard" provides clear, testable criteria that developers and testers can work with confidently.

### Missing Integration Requirements

This pitfall particularly affects brownfield projects where new features must work within existing ecosystems. Teams often focus intensely on new functionality while underestimating integration complexity.

Missing integration requirements surface as unplanned work during development. The team discovers that the new authentication system can't integrate with existing user management, or that API changes break downstream systems that weren't considered during planning.

For brownfield projects, integration requirements deserve as much attention as new functionality. Document existing APIs that must remain compatible, user workflows that must be preserved, and external systems that depend on current behavior.

### Requirements-Epic Misalignment

Sometimes the epic structure evolves separately from requirements, creating disconnects where epics deliver functionality that doesn't map back to stated requirements, or requirements exist that no epic addresses.

This misalignment often results from requirements and epic planning happening at different times or by different people. Without clear traceability, it's easy for the two perspectives to drift apart.

Maintaining a traceability matrix helps ensure every requirement maps to at least one epic and every epic delivers on stated requirements. This doesn't need to be a complex document—even a simple spreadsheet can prevent major misalignments.

### Inadequate Stakeholder Review

PRDs developed in isolation often miss critical perspectives that only emerge during implementation. Technical teams discover requirements conflicts that weren't apparent during planning, or business stakeholders are surprised by delivered functionality that doesn't match their expectations.

The challenge is that stakeholder review takes time, and there's always pressure to move quickly from planning to implementation. However, insufficient review almost always costs more time later through rework and scope clarification.

Structured review processes don't have to be elaborate, but they should ensure both technical feasibility and business alignment before implementation begins. Document review cycles in your change log to maintain transparency about who provided input and when.

---

This guide provides comprehensive direction for creating effective PRDs that drive successful AI-powered development workflows. Choose the appropriate template based on your project context, and use this guidance to ensure your PRD serves as an effective blueprint for development teams and stakeholders.
