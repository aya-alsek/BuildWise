# Data and Information Requirements

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1
**Status:** Draft

## 1. Purpose

This document defines the main information that BuildWise needs to collect, store, manage, and relate to support its core functionality.

It describes information requirements at a conceptual level. Database schema, implementation details, and detailed data structures will be defined later during Analysis and Design.

## 2. Information Scope

BuildWise needs to manage information related to:

* User accounts and contexts
* Projects and project configuration
* Team membership and invitations
* Software Engineering stages and activities
* Project artifacts and documentation
* Progress and completion
* Project evidence
* Project decisions

## 3. User and Account Information

BuildWise shall maintain information required to manage authenticated users, including:

* Basic user and profile information
* Account authentication and recovery information
* User context
* Account status

A user context may include:

* Student
* Recent Graduate
* Trainee
* Independent Learner

User context is used to support onboarding and guidance and does not determine project permissions.

A user may participate in multiple projects, with a different project role in each one.

## 4. Project Information

BuildWise shall maintain information describing each project, including:

* Project name
* Description
* Context
* Type or domain
* Objective
* Working mode
* Selected project approach
* Project status
* Completion information

Each project shall have one Project Owner.

Project information shall remain associated with the Software Engineering work performed within that project.

## 5. Team and Invitation Information

For Team Projects, BuildWise shall maintain information required to manage project participation, including:

* Project Owner
* Team Members
* Team membership
* Project invitations
* Invitation status
* Relationship between an invitation, the invited user, and the project

Team membership and project roles shall apply to a specific project.

## 6. Software Engineering Journey and Progress Information

BuildWise shall maintain information representing the project's progress through the MVP Software Engineering journey:

1. Project Understanding
2. Requirements
3. Analysis
4. Design
5. Implementation
6. Testing
7. Completion

The system shall maintain information about:

* Stages
* Activities
* Activity status and completion
* Current stage
* Next relevant activity
* Stage progress
* Overall project progress
* Remaining work
* Project completion status

The journey shall support iterative work, allowing users to revisit and update previous work.

## 7. Artifact and Documentation Information

BuildWise shall maintain information about engineering artifacts produced during a project.

Artifacts may include:

* Requirements artifacts
* Use cases
* User stories
* Analysis models
* Design artifacts
* Technical decisions
* Test cases
* Project documentation

Each artifact shall be associated with its project and, where applicable, with the relevant Software Engineering stage or activity.

The system shall support relationships between relevant artifacts to help users understand how engineering work is connected.

The exact artifact types and detailed structures will be refined during Analysis and Design.

## 8. Evidence and Decision Information

BuildWise shall maintain information representing evidence of the work performed throughout the project.

Evidence may include:

* Project artifacts
* Engineering activities
* Technical decisions
* Testing evidence
* Deployment-related evidence
* Source-code references
* Project documentation

The system shall also maintain relevant project decisions, including their context and relationship to project work where applicable.

Evidence and decisions shall remain associated with the relevant project and, where applicable, with the artifact or activity they represent.

## 9. Data Relationships and Integrity

At a conceptual level:

* A User may participate in multiple Projects.
* Each Project has one Project Owner.
* A Project may have Team Members and invitations.
* A Project follows a Software Engineering journey.
* A Project contains activities and artifacts.
* Artifacts belong to a Project and may be associated with stages or activities.
* Artifacts may be related to other artifacts.
* Progress is associated with project stages and activities.
* Evidence belongs to a Project and may reference relevant artifacts, activities, or decisions.

BuildWise shall maintain the consistency of these relationships and restrict modification of project information according to the user's authorized project role and permissions.

Detailed validation and integrity rules will be refined during Analysis and Design.

## 10. Data Privacy and Lifecycle

BuildWise shall protect user and project information according to applicable access permissions.

Project information may be updated throughout the Software Engineering journey. Project completion shall not remove the project's artifacts, evidence, or relevant engineering information.

Detailed privacy, retention, deletion, and archival rules will be refined as operational requirements are established.

## 11. MVP Scope

The MVP requires information management sufficient to support:

* User accounts and contexts
* Project creation and configuration
* Solo and Team projects
* Team membership and invitations
* Software Engineering stages and activities
* Core artifacts and documentation
* Artifact relationships
* Progress tracking
* Project completion
* Project evidence and decisions

Advanced analytics, complex version history, real-time collaboration data, organizational reporting, and advanced AI-generated insights are outside the current MVP scope.

## 12. Relationship to Analysis and Design

This document defines **what information BuildWise needs to manage**, not how it will be implemented.

The following will be defined during later Analysis and Design:

* Conceptual data model and entity relationships
* Detailed data attributes
* Database schema and storage design
* Data validation and integrity rules
