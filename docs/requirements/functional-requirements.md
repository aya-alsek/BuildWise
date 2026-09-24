# Functional Requirements

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1

## 1. Purpose

This document defines the functional requirements of BuildWise.

Functional requirements describe what the system shall do from the user's perspective without specifying implementation technologies or internal design decisions.

Requirements are grouped by major system capabilities.

---

# 2. Account and Access

## FR-ACC-01 — User Registration

The system shall allow a Visitor to create a BuildWise account using their required registration information.

The system shall:

* Validate the provided registration information.
* Prevent registration using an email address already associated with an account.
* Confirm successful account creation.
* Provide appropriate feedback when registration fails.

---

## FR-ACC-02 — User Login

The system shall allow a registered User to log in using their account credentials.

The system shall:

* Validate the provided credentials.
* Grant access when the credentials are valid.
* Reject invalid credentials.
* Provide appropriate feedback when authentication fails.

---

## FR-ACC-03 — User Logout

The system shall allow an authenticated User to log out of their account.

After logout, the system shall prevent access to authenticated features until the User logs in again.

---

## FR-ACC-04 — Account Recovery

The system shall allow a User who cannot access their account to initiate an account recovery process.

The system shall:

* Allow the User to request recovery using their registered email address.
* Provide appropriate recovery instructions.
* Allow the User to regain access after completing the required recovery process.

---

# 3. Onboarding

## FR-ONB-01 — Collect User Context

The system shall allow a newly registered User to provide relevant personal and professional/academic context during onboarding.

The context may include:

* Student
* Recent Graduate
* Trainee
* Independent Learner

---

## FR-ONB-02 — Collect Project Starting Context

The system shall allow the User to provide initial information about their project situation.

This may include:

* Whether the User already has a project idea.
* The purpose of the project.
* The general project type or domain.
* Whether the User intends to work individually or with a team.

---

## FR-ONB-03 — Complete Onboarding

The system shall allow the User to complete the required onboarding information and continue to project setup.

---

# 4. Project Idea

## FR-IDEA-01 — Provide Existing Project Idea

The system shall allow a User to provide an existing project idea.

The User shall be able to provide basic information such as:

* Project title or name
* Initial description
* Problem or goal, when available

---

## FR-IDEA-02 — Clarify Project Idea

The system shall guide the User in clarifying an initial project idea by helping define its basic problem, goal, and context.

---

## FR-IDEA-03 — Explore Project Ideas

The system shall allow a User without an existing project idea to explore possible project directions.

The initial version may provide structured prompts or predefined guidance rather than automated AI-generated ideas.

---

# 5. Project Configuration

## FR-PROJ-01 — Create Project

The system shall allow an authenticated User to create a project.

A project shall have a Project Owner.

---

## FR-PROJ-02 — Define Project Information

The system shall allow the Project Owner to define and update basic project information, including:

* Project name
* Description
* Context
* Type or domain
* Objective

---

## FR-PROJ-03 — Select Working Mode

The system shall allow the Project Owner to select one of the supported working modes:

* Solo
* Team

The selected working mode shall determine the project's team participation model.

---

## FR-PROJ-04 — Access Projects

The system shall allow an authenticated User to view and access projects in which they are authorized to participate.

---

# 6. Team Projects

## FR-TEAM-01 — Create Team Project

The system shall allow a Project Owner to configure a project as a Team Project.

---

## FR-TEAM-02 — Invite Team Members

The system shall allow the Project Owner of a Team Project to invite other users to join the project.

---

## FR-TEAM-03 — Accept Project Invitation

The system shall allow an invited User to accept an invitation to join a Team Project.

---

## FR-TEAM-04 — New User Invitation Flow

The system shall support an invitation flow for a person who does not yet have a BuildWise account.

The person shall be able to create an account and continue the invitation process.

---

## FR-TEAM-05 — Team Membership

The system shall associate accepted members with the corresponding Team Project.

Team members shall be able to access the shared project workspace according to their permissions.

---

# 7. Project Approach

## FR-APP-01 — Understand Project Context

The system shall present relevant project context information before the User selects an engineering approach.

---

## FR-APP-02 — Provide Approach Guidance

The system shall provide basic guidance about possible Software Engineering approaches relevant to the project context.

---

## FR-APP-03 — Select Project Approach

The system shall allow the Project Owner to select the approach used for the project.

The selected approach shall be stored as part of the project's information.

---

# 8. Project Workspace

## FR-WS-01 — Project Workspace

The system shall provide an organized workspace for each project.

The workspace shall provide access to relevant project information, activities, artifacts, progress, and the current Software Engineering stage.

---

## FR-WS-02 — Project Overview

The system shall display an overview of the current project, including relevant project information and current status.

---

## FR-WS-03 — Current Stage

The system shall display the current stage of the Software Engineering journey.

---

## FR-WS-04 — Next Activity

The system shall identify the next relevant activity or action available to the User based on the project's current state.

---

## FR-WS-05 — Project Activities

The system shall display the activities associated with the current project stage.

---

## FR-WS-06 — Team Information

For Team Projects, the system shall display relevant team membership information to authorized project participants.

---

# 9. Software Engineering Journey

## FR-SE-01 — Engineering Journey

The system shall provide a structured Software Engineering journey for each project.

The MVP journey shall include:

1. Project Understanding
2. Requirements
3. Analysis
4. Design
5. Implementation
6. Testing
7. Completion

---

## FR-SE-02 — Stage Guidance

The system shall provide guidance for activities within each supported Software Engineering stage.

Guidance shall explain what the User is expected to do and the purpose of the activity.

---

## FR-SE-03 — Stage Dependencies

The system shall identify relevant dependencies between activities or stages when a previous output is required for subsequent work.

---

# 10. Artifacts and Documentation

## FR-ART-01 — Create Artifact

The system shall allow authorized project participants to create project artifacts associated with Software Engineering activities.

---

## FR-ART-02 — Organize Artifacts

The system shall organize project artifacts according to their relevant project stage or category.

---

## FR-ART-03 — Edit Artifacts

The system shall allow authorized project participants to edit project artifacts.

---

## FR-ART-04 — Requirements Artifacts

The system shall support project artifacts related to requirements, such as:

* Functional requirements
* User stories
* Use cases
* Other relevant requirements documentation

---

## FR-ART-05 — Analysis Artifacts

The system shall support project artifacts related to system analysis.

Examples may include:

* Analysis models
* Process models
* Domain-related models

---

## FR-ART-06 — Design Artifacts

The system shall support project artifacts related to system design.

Examples may include:

* Architecture decisions
* Design models
* Technical decisions

---

## FR-ART-07 — Testing Artifacts

The system shall support project artifacts related to testing.

Examples may include:

* Test cases
* Test results
* Testing documentation

---

## FR-ART-08 — Project Documentation

The system shall allow project participants to create and maintain relevant project documentation.

---

## FR-ART-09 — Artifact Relationships

The system shall allow relevant project artifacts to be associated with related activities or project outputs.

The detailed traceability model shall be defined during Analysis and Design.

---

# 11. Progress Tracking

## FR-PROG-01 — Activity Completion

The system shall allow authorized project participants to mark applicable activities as completed.

---

## FR-PROG-02 — Stage Progress

The system shall display the progress of the project within each Software Engineering stage.

---

## FR-PROG-03 — Overall Progress

The system shall provide an overall indication of project progress.

---

## FR-PROG-04 — Remaining Work

The system shall identify incomplete relevant activities or work remaining in the project.

---

## FR-PROG-05 — Next Step

The system shall indicate the next relevant project activity based on the current project state.

---

# 12. Iteration and Refinement

## FR-ITER-01 — Revisit Previous Work

The system shall allow project participants to return to previously completed activities or stages.

---

## FR-ITER-02 — Update Previous Work

The system shall allow authorized project participants to update previously created project artifacts and information.

---

## FR-ITER-03 — Reflect Changes

The system shall allow updated project work to remain associated with the relevant project activities and artifacts.

Detailed version history is outside the MVP scope.

---

# 13. Project Completion

## FR-COMP-01 — Completion Readiness

The system shall provide an indication of whether the project has completed its required MVP activities and outputs.

---

## FR-COMP-02 — Complete Project

The system shall allow the Project Owner to mark a project as completed when the required completion conditions are satisfied.

---

## FR-COMP-03 — Completion Summary

The system shall provide a summary of the project's completed Software Engineering activities and outputs.

---

# 14. Project Evidence

## FR-EVID-01 — Project Evidence

The system shall provide an overview of the evidence produced during the project.

Evidence may include:

* Requirements
* Analysis artifacts
* Design artifacts
* Project documentation
* Source code references
* Testing evidence
* Deployment information
* Important project decisions

---

## FR-EVID-02 — Artifact Evidence

The system shall associate relevant project artifacts with the project's evidence.

---

## FR-EVID-03 — Engineering Activity Evidence

The system shall associate completed Software Engineering activities with their relevant outputs or evidence.

---

## FR-EVID-04 — Project Decisions

The system shall allow important project decisions to be recorded as part of the project's evidence.

---

## FR-EVID-05 — Evidence Overview

The system shall provide an organized overview of the project's accumulated evidence.

---

**Note:** Requirements may be refined during subsequent Requirements Engineering, Analysis, Design, and validation activities.
