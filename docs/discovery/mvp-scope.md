# MVP Scope

## 1. Purpose

This document defines the initial Minimum Viable Product (MVP) scope for BuildWise.

The purpose of the MVP is to identify the smallest meaningful version of BuildWise that can deliver and validate its core product value.

The MVP focuses on helping individual Software Engineering learners turn a software project idea into a structured and connected Software Engineering process.

This document defines product boundaries at a high level. It does not define detailed functional requirements, system behavior, technical implementation, or user interface specifications. These will be defined later during Requirements Engineering and subsequent development phases.

---

## 2. MVP Objective

The primary objective of the BuildWise MVP is to validate whether the platform can help a user:

* Start with a software project idea.
* Understand what should be done throughout the project.
* Follow a structured Software Engineering journey.
* Produce meaningful project artifacts.
* Understand why each activity is performed.
* Connect activities and artifacts across the project.
* Track project progress.
* Revisit and refine previous work when necessary.
* Complete the project with organized evidence of the work performed.

The MVP should demonstrate the core BuildWise concept without attempting to implement the full long-term product vision.

---

## 3. Core MVP User

The initial MVP focuses on:

> **Individual Software Engineering learners building real software projects.**

This may include users such as:

* Final-year students working on graduation projects.
* Recent Software Engineering graduates.
* Software Engineering trainees.
* Independent learners building practical projects.

These contexts may differ, but the MVP focuses on their shared need to apply Software Engineering practices while building a real project.

Organizational users such as universities, training organizations, trainers, and mentors are considered future product contexts and are not part of the initial MVP user scope.

---

## 4. MVP User Journey

The core MVP journey is:

**Account Creation / Login → Onboarding → Project Idea → Project Configuration → Solo / Team → Project Approach → Project Workspace → Software Engineering Journey → Artifacts & Documentation → Progress Tracking → Iteration → Project Completion → Project Evidence**

The exact screens, workflows, permissions, and system behavior will be defined later.

---

# 5. MVP Capabilities

## 5.1 Account and Access

Users should be able to:

* Create an account.
* Log in.
* Log out.
* Access their projects and saved work.

Authentication and security details will be defined during Requirements Engineering.

---

## 5.2 Onboarding

BuildWise should collect enough initial information to understand the user's context and support project setup.

Potential information may include:

* User context, such as student, graduate, trainee, or independent learner.
* Field of study or professional field.
* University or organization, where relevant.
* Whether the user already has a project idea.
* Whether the user is working individually or with a team.

The onboarding process should remain focused on information that can meaningfully affect the user's BuildWise experience.

Detailed data requirements will be defined later.

---

## 5.3 Project Idea

BuildWise should support users who:

### Have a Project Idea

The user can provide and clarify the initial project idea.

The platform may help the user identify basic project context such as:

* The problem being addressed.
* Intended users.
* General project goal.
* General project type or domain.

### Do Not Have a Project Idea

BuildWise should provide a basic way to help the user explore and develop a suitable project direction.

Possible mechanisms may include:

* Guided questions.
* Project categories.
* Example project directions.
* Project prompts.

The exact mechanism will be determined during Requirements Engineering and MVP design.

Advanced AI-based idea generation is not required for the initial MVP.

---

## 5.4 Project Configuration

The user should be able to create and configure a project.

Initial project information may include:

* Project name.
* Project description.
* Project context.
* Project type or domain.
* Project objective.
* Working mode.

The MVP should collect only the information necessary to establish the project context and begin the engineering journey.

---

## 5.5 Solo and Team Projects

A project should support two working modes:

* Solo.
* Team.

For Team projects, the initial MVP may support:

* Creating a team.
* Assigning the project to the team.
* Inviting members.
* Accepting invitations.
* Joining the shared project workspace.

The initial team model should remain simple.

Advanced collaboration features, complex permissions, and enterprise-level team management are outside the initial MVP.

---

## 5.6 Project Approach


BuildWise should help the user understand and select an appropriate Software Engineering approach based on the project's context.

The guidance may consider factors such as:

* Project characteristics.
* Project size.
* Solo or team context.
* Project goals.
* Expected development process.

The MVP may provide simplified guidance or recommendations rather than a highly advanced methodology engine.

The user remains responsible for the final engineering decisions.

---

## 5.7 Project Workspace

Each project should have a central workspace where the user can manage the project's Software Engineering journey.

At a high level, the workspace should provide access to:

* Project information.
* Current project stage.
* Project activities.
* Project artifacts.
* Progress information.
* Team information when applicable.
* Relevant guidance.

The detailed workspace structure will be defined later.

---

## 5.8 Software Engineering Journey

### MVP — Core Capability

The Software Engineering journey is the central capability of the BuildWise MVP.

The platform should guide users through a structured journey that may include:

**Project Understanding → Requirements → Analysis → Design → Implementation → Testing → Completion**

The journey should help users understand:

* What they are working on.
* Why the activity is needed.
* What should be produced.
* How the activity relates to previous work.
* What should happen next.

The journey should not be treated as a completely rigid sequence.

Users may need to revisit previous stages when new information, requirements, or feedback are discovered.

For example:

**Testing → Feedback → Requirements Update → Design Update → Implementation → Testing**

Detailed stages and activities will be defined during Requirements Engineering.

---

## 5.9 Artifacts and Documentation

### MVP — Core Capability

Users should be able to create, organize, and maintain meaningful project artifacts throughout the engineering journey.

Potential artifacts may include:

* Requirements.
* Use Cases.
* User Stories.
* Analysis models.
* Design artifacts.
* Technical decisions.
* Test cases.
* Project documentation.

The final artifact set is not defined by this document and will be determined during Requirements Engineering.

The MVP should establish the concept that project artifacts are connected outputs of the Software Engineering process rather than isolated documents.

---

## 5.10 Progress Tracking


Users should be able to understand:

* Their current project stage.
* Completed activities.
* Remaining activities.
* The next recommended activity.
* Overall project progress.

Progress tracking should support the core BuildWise goal of reducing uncertainty about what to do next.

---

## 5.11 Iteration and Refinement

### MVP — Simplified

Users should be able to revisit and update previous project work when necessary.

For example:

**Requirements → Analysis → Design → Implementation → Testing**

If a problem is discovered during testing, the user may return to an earlier activity and refine the relevant artifacts.

The MVP does not need a complex change-management or version-control system for this capability.

---

## 5.12 Project Completion

BuildWise should provide a clear project completion state based on the relevant project activities and expected outputs.

Completion should not be defined only by whether the software runs successfully.

The completed project should reflect the engineering work performed throughout the project journey.

Detailed completion criteria will be defined during Requirements Engineering.

---

## 5.13 Project Evidence

BuildWise should preserve an organized representation of the user's project work.

Project evidence may include:

* Requirements.
* Analysis artifacts.
* Design artifacts.
* Documentation.
* Source code references.
* Testing information.
* Deployment information.
* Relevant project decisions.

The purpose is to help users preserve evidence of practical Software Engineering experience gained through the project.

---

# 6. MVP Boundaries

The MVP focuses on the following core value:

> **Guiding an individual Software Engineering learner through a structured and connected project-building process while helping them produce meaningful engineering artifacts and practical project evidence.**

The MVP does not attempt to become a complete development ecosystem.

The first release should prioritize the engineering workflow and project experience over advanced integrations and automation.

---

# 7. Out of Scope for the Initial MVP

The following capabilities are considered outside the initial MVP scope:

### Organizational Features

* University dashboards.
* Training organization management.
* Trainer and mentor management.
* Academic supervision workflows.
* Enterprise-level project management.

### Advanced AI Capabilities

* Advanced AI project generation.
* Automated requirements analysis.
* Automated artifact review.
* Automated design validation.
* Advanced AI code review.

AI may be considered later or used in limited ways where it directly supports the MVP experience.

### Development Tool Integrations

* GitHub integration.
* Automated repository analysis.
* IDE integration.
* Automated deployment integrations.

### Advanced Collaboration

* Complex permission systems.
* Advanced team management.
* Real-time collaborative editing.
* Enterprise collaboration workflows.

### Public Platform Features

* Public project marketplace.
* Public project showcase.
* Advanced project sharing.

### Platform Analytics

Advanced product analytics and statistics are not part of the initial MVP implementation.

Examples of future platform statistics may include:

* Number of registered users.
* Number of projects.
* Number of completed projects.
* User distribution by field or context.
* University and organization representation.
* Solo versus team project distribution.
* Project type distribution.

These statistics are more meaningful after BuildWise begins receiving real users and real project data.

---

# 8. Future Product Direction

The MVP provides the foundation for potential future expansion.

Future versions may include:

* Advanced AI-assisted Software Engineering guidance.
* GitHub and development-tool integrations.
* Advanced code assistance and review.
* More advanced team collaboration.
* Trainer and mentor workflows.
* Training organization support.
* University and academic program support.
* Public project portfolios and showcases.
* Advanced analytics and reporting.
* Support for broader software project types and development environments.

These possibilities represent future product direction and are not commitments for the initial release.

---

# 9. MVP Validation Goal

The MVP should help validate the following product hypothesis:

> **Software Engineering learners can benefit from a platform that guides them through a structured and connected engineering journey while they build a real software project.**

The MVP should help us learn:

* Whether users understand the BuildWise journey.
* Whether the guidance reduces uncertainty about what to do next.
* Whether users can apply Software Engineering concepts through the workflow.
* Whether users can produce meaningful project artifacts.
* Whether users perceive value in having their project work organized and connected.
* Which parts of the journey require improvement or simplification.

The results of using the MVP should inform future product iterations.

---

# 10. Relationship to Requirements Engineering

This MVP Scope defines **what is included in the first product version at a high level**.

It does not yet define exactly how the system should behave.

The next phase is to translate the MVP scope into detailed requirements, including:

* Functional Requirements.
* Non-Functional Requirements.
* User Roles.
* Business Rules.
* Data Requirements.
* Constraints and Assumptions.
* External Interfaces.

These requirements will form the basis for the Software Requirements Specification (SRS).

---

# 11. Discovery and Product Status

**Version:** 0.1

**Status:** Initial MVP Scope

This MVP scope represents the current product direction based on the initial Product Discovery work.

The scope may be refined if new evidence, user validation, or requirements analysis identifies important changes.

The MVP should remain intentionally focused so that BuildWise can be developed, tested, evaluated, and improved iteratively.
