# Software Requirements Specification

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1
**Status:** Draft

---

## 1. Introduction

### 1.1 Purpose

This document specifies the software requirements for BuildWise.

It consolidates the main requirements identified during the Requirements Engineering phase and provides a single reference for understanding what BuildWise is expected to provide.

Detailed requirements are maintained in their respective requirement documents within `docs/requirements/`.

### 1.2 Scope

BuildWise is a practical Software Engineering environment that helps learners turn Software Engineering knowledge into practical project experience.

The platform guides users through a structured and connected Software Engineering journey while helping them create, organize, refine, and track project artifacts and evidence.

The MVP focuses on individual Software Engineering learners, including final-year students, recent graduates, trainees, and independent learners.

### 1.3 Document Overview

This SRS covers:

* Product overview and goals
* Users and system actors
* Functional requirements
* Non-functional requirements
* Business rules
* Data and information requirements
* External interfaces
* Constraints and assumptions
* MVP scope
* References and terminology

---

## 2. Product Overview

### 2.1 BuildWise Overview

BuildWise helps learners move from Software Engineering knowledge to practical project experience by providing a structured project environment.

The platform focuses on helping users understand:

* What they should do
* Why each activity is performed
* What output should be produced
* How different activities and artifacts are connected
* What work has been completed
* What should be done next

BuildWise supports an iterative approach, allowing users to revisit and refine previous work as their project evolves.

### 2.2 Product Goals

The main goals of BuildWise are to:

1. Connect Software Engineering knowledge with practical project work.
2. Provide a structured Software Engineering journey.
3. Help users produce meaningful engineering artifacts.
4. Connect related activities and artifacts.
5. Improve confidence in Software Engineering decisions.
6. Help learners build practical experience and organized project evidence.

### 2.3 Core Value

BuildWise helps Software Engineering learners turn knowledge into practical experience by guiding them through a structured and connected Software Engineering journey while they build real projects.

### 2.4 High-Level System Context

At a high level, a user interacts with BuildWise through a web interface to:

* Create and manage projects
* Configure project context
* Work individually or as part of a team
* Follow the Software Engineering journey
* Create and manage project artifacts
* Track progress
* Revisit and refine previous work
* Complete the project
* Organize project evidence

External services such as email communication and externally hosted project resources may support the platform where applicable.

---

## 3. Users and Actors

### 3.1 Visitor

A Visitor is an unauthenticated person interacting with BuildWise.

A Visitor may:

* View the landing page
* Access registration
* Access login

A Visitor cannot access private user or project information.

### 3.2 User

A User is an authenticated BuildWise account holder.

A User may:

* Manage their account
* Create and access projects
* Participate in projects according to project-level permissions
* Follow the Software Engineering journey
* Create and manage permitted artifacts
* Track and update project progress

### 3.3 Project Owner

The Project Owner is responsible for a project.

The Project Owner may:

* Create and configure the project
* Define project information and objectives
* Manage project work
* Invite team members
* Manage project artifacts
* Track project progress
* Complete the project

For a Team Project, the Project Owner also acts as the Team Leader.

### 3.4 Team Member

A Team Member is an authenticated user who participates in a Team Project without being its Project Owner.

A Team Member may access and contribute to shared project work according to the permissions defined for the project.

### 3.5 User Contexts

BuildWise may identify a user's context during onboarding, such as:

* Student
* Recent Graduate
* Trainee
* Independent Learner

These contexts are used to provide relevant guidance and do not determine project permissions.

---

## 4. Functional Requirements

The following requirements describe the main capabilities BuildWise shall provide.

### 4.1 Account and Access

* **FR-ACC-01:** User Registration
* **FR-ACC-02:** User Login
* **FR-ACC-03:** User Logout
* **FR-ACC-04:** Account Recovery

### 4.2 Onboarding

* **FR-ONB-01:** Collect User Context
* **FR-ONB-02:** Collect Project Starting Context
* **FR-ONB-03:** Complete Onboarding

### 4.3 Project Idea

* **FR-IDEA-01:** Provide Existing Project Idea
* **FR-IDEA-02:** Clarify Project Idea
* **FR-IDEA-03:** Explore Project Ideas

### 4.4 Project Configuration

* **FR-PROJ-01:** Create Project
* **FR-PROJ-02:** Define Project Information
* **FR-PROJ-03:** Select Working Mode
* **FR-PROJ-04:** Access Projects

### 4.5 Team Projects

* **FR-TEAM-01:** Create Team Project
* **FR-TEAM-02:** Invite Team Members
* **FR-TEAM-03:** Accept Project Invitation
* **FR-TEAM-04:** Support New User Invitation Flow
* **FR-TEAM-05:** Manage Team Membership

### 4.6 Project Approach

* **FR-APP-01:** Understand Project Context
* **FR-APP-02:** Provide Approach Guidance
* **FR-APP-03:** Select Project Approach

### 4.7 Project Workspace

* **FR-WS-01:** Provide Project Workspace
* **FR-WS-02:** Provide Project Overview
* **FR-WS-03:** Display Current Stage
* **FR-WS-04:** Display Next Activity
* **FR-WS-05:** Display Project Activities
* **FR-WS-06:** Display Team Information

### 4.8 Software Engineering Journey

BuildWise shall provide a structured Software Engineering journey consisting of:

1. Project Understanding
2. Requirements
3. Analysis
4. Design
5. Implementation
6. Testing
7. Completion

The journey shall provide guidance and stage dependencies where applicable.

* **FR-SE-01:** Provide Engineering Journey
* **FR-SE-02:** Provide Stage Guidance
* **FR-SE-03:** Provide Stage Dependencies

The journey is iterative, allowing users to revisit earlier stages when project changes require refinement.

### 4.9 Artifacts and Documentation

* **FR-ART-01:** Create Artifact
* **FR-ART-02:** Organize Artifacts
* **FR-ART-03:** Edit Artifacts
* **FR-ART-04:** Manage Requirements Artifacts
* **FR-ART-05:** Manage Analysis Artifacts
* **FR-ART-06:** Manage Design Artifacts
* **FR-ART-07:** Manage Testing Artifacts
* **FR-ART-08:** Manage Project Documentation
* **FR-ART-09:** Maintain Artifact Relationships

Artifacts may include requirements, analysis models, design artifacts, testing information, technical decisions, and project documentation.

### 4.10 Progress Tracking

* **FR-PROG-01:** Track Activity Completion
* **FR-PROG-02:** Track Stage Progress
* **FR-PROG-03:** Track Overall Progress
* **FR-PROG-04:** Display Remaining Work
* **FR-PROG-05:** Display Next Step

### 4.11 Iteration and Refinement

* **FR-ITER-01:** Revisit Previous Work
* **FR-ITER-02:** Update Previous Work
* **FR-ITER-03:** Reflect Changes

Users shall be able to revisit and refine previous project work without permanently locking completed stages.

### 4.12 Project Completion

* **FR-COMP-01:** Assess Completion Readiness
* **FR-COMP-02:** Complete Project
* **FR-COMP-03:** Provide Completion Summary

Project completion shall consider the completion of relevant activities and outputs rather than only whether the software is operational.

### 4.13 Project Evidence

* **FR-EVID-01:** Manage Project Evidence
* **FR-EVID-02:** Manage Artifact Evidence
* **FR-EVID-03:** Record Engineering Activity Evidence
* **FR-EVID-04:** Record Project Decisions
* **FR-EVID-05:** Provide Evidence Overview

Project evidence may include requirements, analysis, design, documentation, source-code references, testing information, deployment information, and relevant engineering decisions.

Detailed functional requirements are maintained in `docs/requirements/functional-requirements.md`.

---

## 5. Non-Functional Requirements

BuildWise shall satisfy the following quality requirements.

### 5.1 Usability

The system should provide:

* Clear navigation
* Understandable guidance
* Consistent interaction and interface patterns

### 5.2 Performance

The system should provide:

* Responsive interaction
* Efficient project loading

Specific measurable performance targets will be defined when deployment and expected usage are better understood.

### 5.3 Security

The system shall provide:

* Secure authentication
* Password protection
* Authorization based on the authenticated user's project role and permissions
* Input validation

An authenticated user shall only be able to access or modify private project data for projects in which they have the required permissions.

### 5.4 Reliability and Data Integrity

The system should support:

* Persistent project data
* Data consistency
* Appropriate error handling

### 5.5 Maintainability

The system should support:

* Modular structure
* Appropriate technical and project documentation

### 5.6 Compatibility and Accessibility

The system should support:

* Responsive design
* Modern web browsers
* Basic accessibility practices

### 5.7 Scalability

The system architecture should consider future growth in users, projects, and platform usage.

### 5.8 Privacy

The system shall protect:

* Project information
* User data
* Private project access

Detailed NFRs are maintained in `docs/requirements/non-functional-requirements.md`.

---

## 6. Business Rules

BuildWise shall follow the following high-level business rules.

### 6.1 User and Account Rules

* BuildWise has one authenticated account type: User.
* User contexts such as Student or Recent Graduate do not determine permissions.
* Each account belongs to one User.

### 6.2 Project Rules

* Each project has exactly one Project Owner.
* A User may participate in multiple projects.
* A User may have different project roles in different projects.
* Each project operates in either Solo or Team mode.
* A Solo Project has one Owner.
* A Team Project has an Owner and may include Team Members.
* The Project Owner acts as Team Leader for a Team Project.

### 6.3 Team Membership Rules

* A User becomes a Team Member after accepting a project invitation.
* Each invitation is associated with a specific project and invited person.
* Project access is determined by the user's project role and permissions.

### 6.4 Software Engineering Journey Rules

* Each project follows the BuildWise Software Engineering journey.
* Stage progress is based on relevant activities and outputs.
* Users may revisit and update previous work.

### 6.5 Artifact Rules

* Each artifact belongs to a project.
* Artifacts are associated with relevant Software Engineering stages or activities where applicable.
* Only users with the required permissions may create or modify project artifacts.
* Artifact updates preserve their project and engineering context.

### 6.6 Completion Rules

* A project is ready for completion when required MVP activities and outputs have been completed.
* The Project Owner is responsible for marking a project as completed.
* Completed projects retain their artifacts and evidence.

### 6.7 Privacy Rules

* Project data is private by default.
* Private project data may only be accessed by users with the required permissions.
* User context does not grant access to project data.

Detailed business rules are maintained in `docs/requirements/business-rules.md`.

---

## 7. Data and Information Requirements

BuildWise shall manage the information required to support its core functionality.

### 7.1 User and Account Information

The system shall maintain information required for:

* User accounts
* Authentication
* User context
* Account-related information

### 7.2 Project Information

The system shall maintain:

* Project identity
* Description
* Context
* Type/domain
* Objective
* Working mode
* Project ownership

### 7.3 Team and Invitation Information

For Team Projects, the system shall maintain information related to:

* Team membership
* Project invitations
* Invitation status
* Project roles

### 7.4 Software Engineering Journey and Progress

The system shall maintain information related to:

* Current stage
* Activities
* Activity completion
* Stage progress
* Overall progress
* Remaining work
* Next steps

### 7.5 Artifact and Documentation Information

The system shall maintain:

* Artifact identity and content
* Artifact type
* Related project
* Related Software Engineering stage/activity where applicable
* Artifact relationships
* Documentation

### 7.6 Evidence and Decision Information

The system shall support information related to:

* Project evidence
* Artifact evidence
* Engineering activity evidence
* Project decisions
* Decision context where applicable

### 7.7 Data Relationships and Integrity

Data shall maintain the relationships required to preserve project, user, team, artifact, activity, and evidence context.

The following will be refined during later Analysis and Design activities:

* Conceptual data model and entity relationships
* Detailed data attributes
* Database schema and storage design
* Data validation and integrity rules

Requirements traceability will be maintained as needed across requirements, design, implementation, and testing activities.

Detailed data requirements are maintained in `docs/requirements/data-information-requirements.md`.

---

## 8. External Interfaces

### 8.1 User Interface

BuildWise shall provide a web-based user interface through which users can:

* Register and log in
* Configure projects
* Navigate the Software Engineering journey
* Manage artifacts
* Track progress
* Review project evidence

Detailed visual design and implementation decisions are outside the scope of this requirements document.

### 8.2 Email Interface

Email communication may be used for system-related communication such as:

* Account recovery
* Project invitations
* Other required user notifications

Specific email service implementation will be defined during later design and implementation activities.

### 8.3 External Project References

BuildWise shall allow users to include manually provided external references as part of project evidence, without requiring direct integration with external platforms.

### 8.4 Future External Interfaces

Potential future integrations may include:

* GitHub or other source-control platforms
* AI services
* Deployment platforms
* Additional external development services

These integrations are outside the current MVP requirements unless explicitly added later.

Detailed interface requirements are maintained in `docs/requirements/external-interfaces.md`.

---

## 9. Constraints and Assumptions

BuildWise development is subject to the constraints and assumptions identified during Requirements Engineering.

These include:

* The MVP focuses on core individual learner functionality.
* Basic Team Project functionality is included within the current scope.
* Advanced collaboration capabilities are outside the MVP.
* Advanced organizational features are outside the MVP.
* Advanced AI capabilities are outside the MVP.
* Direct GitHub, IDE, deployment, and similar integrations are outside the MVP.
* Advanced permissions and real-time collaboration are outside the MVP.
* Future platform capabilities may require additional requirements and design work.

Detailed constraints and assumptions are maintained in `docs/requirements/constraints-and-assumptions.md`.

---

## 10. MVP Scope

### 10.1 In Scope

The MVP shall support the core journey:

**Account Creation/Login → Onboarding → Project Idea → Project Configuration → Solo/Team → Project Approach → Project Workspace → Software Engineering Journey → Artifacts/Documentation → Progress Tracking → Iteration → Completion → Evidence**

Core MVP capabilities include:

* Account and access management
* Basic onboarding
* Project creation and configuration
* Solo and Team Projects
* Basic team invitations and membership
* Project approach guidance
* Project workspace
* Structured Software Engineering journey
* Core engineering artifacts
* Progress tracking
* Iteration and refinement
* Project completion
* Organized project evidence

### 10.2 Out of Scope

The following are outside the current MVP scope:

* Organizational user management
* Advanced AI features
* Direct GitHub/repository integration
* IDE integration
* Direct deployment integration
* Advanced real-time collaboration
* Advanced team permissions
* Public marketplace or advanced showcase capabilities
* Platform analytics based on real user activity

### 10.3 Future Direction

Future versions may expand BuildWise to support:

* Advanced AI-assisted engineering guidance and artifact review
* Code explanation and review
* GitHub and development-tool integrations
* Advanced collaboration
* Mentors and trainers
* Universities and training organizations
* Public project portfolios and showcase features
* Platform analytics after sufficient real usage data exists
* Additional project types and technical guidance

MVP scope may be refined through iterative development and future validation.

---

## 11. References and Glossary

### 11.1 Requirements References

The following documents provide detailed requirements supporting this SRS:

* `docs/requirements/user-roles-and-actors.md`
* `docs/requirements/functional-requirements.md`
* `docs/requirements/non-functional-requirements.md`
* `docs/requirements/business-rules.md`
* `docs/requirements/constraints-and-assumptions.md`
* `docs/requirements/data-information-requirements.md`
* `docs/requirements/external-interfaces.md`

Related product-level documents are maintained under:

* `docs/discovery/`

### 11.2 Glossary

**BuildWise:** The Software Engineering learning and practical project environment being developed.

**Software Engineering (SE):** The systematic application of engineering principles to software development and maintenance.

**SDLC:** Software Development Life Cycle.

**SRS:** Software Requirements Specification.

**Functional Requirement:** A requirement describing what the system shall do.

**Non-Functional Requirement:** A requirement describing a quality, constraint, or characteristic of the system.

**Artifact:** A documented output produced or maintained during a Software Engineering activity.

**Project Owner:** The User responsible for a specific BuildWise project.

**Team Member:** A User participating in a Team Project without being its Project Owner.

**Team Project:** A project in which the Project Owner works with one or more Team Members.

**MVP:** Minimum Viable Product; the smallest meaningful version of BuildWise intended to validate the product's core value.

---
