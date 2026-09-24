# Data and Information Requirements

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1
**Status:** Draft

## 1. Purpose

This document defines the main information that BuildWise needs to collect, store, manage, and relate in order to support its core functionality.

The purpose is to describe the information requirements at a conceptual level without defining the database schema, implementation technology, or detailed data structures.

The detailed data model and database design will be defined later during the Analysis and Design phases.

---

## 2. Information Requirements Scope

BuildWise needs to manage information related to:

1. User accounts and contexts
2. Projects
3. Project teams and invitations
4. Project approach and configuration
5. Software Engineering stages and activities
6. Project artifacts and documentation
7. Progress and completion
8. Project evidence
9. Project decisions and engineering history

---

## 3. User and Account Information

BuildWise shall maintain information required to identify and manage authenticated users.

### 3.1 User Information

The system shall maintain information such as:

* User identity and basic profile information
* Account credentials and authentication-related information
* User context
* Account status
* Information required for account recovery

### 3.2 User Context

A user's context may include:

* Student
* Recent Graduate
* Trainee
* Independent Learner

User context is used to support relevant onboarding and guidance. It shall not determine project permissions.

### 3.3 User Relationships

The system shall be able to associate users with the projects in which they participate.

A user may participate in multiple projects, and the user's project role may differ between projects.

---

## 4. Project Information

BuildWise shall maintain information describing each project.

A project may include:

* Project name
* Project description
* Project context
* Project type or domain
* Project objective
* Working mode
* Selected project approach
* Project status
* Completion information

Each project shall be associated with its Project Owner.

Project information shall remain connected to the Software Engineering work performed within that project.

---

## 5. Team and Invitation Information

For Team Projects, BuildWise shall maintain information required to manage project participation.

This includes:

* Project team membership
* Project Owner
* Team Members
* Project invitations
* Invitation status
* Relationship between an invitation, the invited user, and the project

Team membership shall be associated with a specific project.

A user's participation in one project shall not automatically determine their role in another project.

---

## 6. Project Configuration Information

BuildWise shall maintain the information used to configure a project and determine its initial working context.

This may include:

* Project context
* Project type or domain
* Project objective
* Working mode
* Selected project approach
* Initial project idea or problem description

The system shall preserve this information as part of the project's overall engineering context.

---

## 7. Software Engineering Journey Information

BuildWise shall maintain information representing the project's progress through its Software Engineering journey.

For the MVP, the journey includes:

1. Project Understanding
2. Requirements
3. Analysis
4. Design
5. Implementation
6. Testing
7. Completion

The system shall maintain information about:

* Project stage
* Stage activities
* Activity status
* Activity completion
* Relationships between activities where applicable
* Current project stage
* Next relevant activity

The journey shall support iterative work, allowing users to revisit and update previous stages.

---

## 8. Artifact and Documentation Information

BuildWise shall maintain information about the engineering artifacts produced during a project.

Artifacts may include:

* Requirements artifacts
* Use cases
* User stories
* Analysis models
* Design artifacts
* Technical decisions
* Test cases
* Project documentation

For each artifact, the system shall be able to maintain information needed to:

* Identify the artifact
* Associate it with its project
* Associate it with the relevant Software Engineering stage or activity
* Store its content or reference
* Track its current state
* Maintain relevant relationships with other artifacts

The exact artifact types and detailed structures will be refined during later Analysis and Design work.

---

## 9. Artifact Relationships and Traceability Information

BuildWise shall maintain relationships between relevant engineering artifacts.

These relationships may connect artifacts such as:

* Requirements to use cases
* Requirements to analysis artifacts
* Requirements to design artifacts
* Design artifacts to implementation-related information
* Requirements or design decisions to test cases

The purpose is to help users understand how engineering work is connected across the project.

Detailed traceability mechanisms will be defined during later Analysis and Design phases.

---

## 10. Progress Information

BuildWise shall maintain information required to represent project progress.

This includes:

* Activity completion status
* Stage progress
* Overall project progress
* Remaining work
* Current next step
* Project completion status

Progress information shall be associated with the relevant project activities and Software Engineering stages.

---

## 11. Project Evidence Information

BuildWise shall maintain information that represents the evidence produced throughout the project.

Evidence may include:

* Project artifacts
* Engineering activities
* Technical decisions
* Testing evidence
* Deployment-related evidence
* Source-code references
* Project documentation

Evidence shall remain associated with the relevant project and, where applicable, with the artifact or engineering activity it represents.

The purpose of project evidence is to provide an organized representation of the work performed throughout the Software Engineering journey.

---

## 12. Project Decision and Engineering History Information

BuildWise shall maintain relevant information about important project decisions and changes.

This may include:

* Decision made
* Context or reason for the decision
* Related project activity or artifact
* Resulting change where applicable

This information supports the user's ability to understand and document how the project evolved.

The MVP does not require advanced version control or a complete historical versioning system.

---

## 13. Data Relationships

At a conceptual level, BuildWise information shall maintain relationships such as:

* A User may participate in multiple Projects.
* Each Project has one Project Owner.
* A Project may contain Team Members.
* A Project may have project invitations.
* A Project follows a Software Engineering journey.
* A Project contains activities and artifacts.
* Artifacts belong to a Project and may be associated with specific stages or activities.
* Artifacts may be related to other artifacts.
* Progress information is associated with project activities and stages.
* Evidence belongs to a Project and may reference artifacts, activities, decisions, or other project outputs.
* Project decisions are associated with the project and may be related to relevant artifacts or activities.

These relationships describe information dependencies at the requirements level. They do not represent the final database structure.

---

## 14. Data Integrity and Consistency Requirements

BuildWise shall maintain the consistency of project information.

At minimum:

* Project information shall remain associated with the correct project.
* Artifacts shall remain associated with their project.
* Project roles and memberships shall be associated with the correct project.
* Progress information shall correspond to the relevant activities and stages.
* Evidence shall remain associated with the work it represents.
* Users shall not be able to create or modify information outside their permitted project access.
* Information required for project completion shall remain available after project completion.

Detailed validation and integrity rules will be refined during Analysis and Design.

---

## 15. Data Privacy

Project and user information may contain private or sensitive information.

BuildWise shall therefore maintain appropriate access restrictions for private information according to the user's authenticated project role and permissions.

Project visibility and public-sharing behavior will be refined as the product evolves and will be aligned across the relevant requirements and business rules in a later iteration.

---

## 16. Data Lifecycle

BuildWise information may pass through different states during a project's lifecycle.

For example:

**Created → Updated → Used/Referenced → Completed → Retained**

Users may revisit and update project information and artifacts during the Software Engineering journey.

Project completion shall not automatically remove the project's artifacts, evidence, or relevant engineering information.

Specific retention, deletion, archival, and recovery policies will be defined later when operational and deployment requirements are established.

---

## 17. MVP Scope

The MVP requires information management sufficient to support:

* User accounts
* User contexts
* Project creation and configuration
* Solo and Team projects
* Team membership and invitations
* Software Engineering stages and activities
* Core project artifacts
* Artifact relationships
* Progress tracking
* Project completion
* Project evidence
* Project decisions

Advanced data capabilities such as:

* Advanced analytics
* Complex version history
* Real-time collaboration data
* Advanced audit systems
* Advanced AI-generated project insights
* Organizational reporting data
* University or training-organization data

are outside the current MVP scope.

---

## 18. Relationship to Later Design

This document defines **what information BuildWise needs to manage**, not how that information will be implemented.

The following will be defined during later Analysis and Design activities:

* Conceptual data model
* Entity relationships
* Detailed attributes
* Database schema
* Data validation rules
* Data storage structure
* Data access mechanisms
* Detailed traceability model

This separation allows the requirements to remain stable while the technical design evolves.

---

## 19. Status

This document represents the initial Data and Information Requirements for BuildWise and may be refined as requirements are validated and the system moves into Analysis and Design.
