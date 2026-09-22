# High-Level User Journey

## 1. Purpose

This document describes the initial high-level journey of a BuildWise user from entering the platform to completing a software project.

The purpose is to understand the overall user experience and the major stages of interaction with BuildWise before defining detailed MVP features or system requirements.

This journey is intentionally high-level. Detailed screens, features, permissions, workflows, and system behavior will be defined later during MVP definition and Requirements Engineering.

---

## 2. Journey Overview

The initial BuildWise user journey is:

**Landing Page → Account Creation / Login → Onboarding → Project Context → Project Setup → Project Approach → Project Workspace → Software Engineering Journey → Project Completion → Project Evidence / Optional Sharing**

The journey may vary depending on the user's context, whether they already have a project idea, and whether they are working individually or as part of a team.

---

## 3. Stage 1 — Landing Page

The user first encounters BuildWise through the landing page.

The landing page should help the user understand:

* What BuildWise is.
* Who it is intended for.
* What problem it helps address.
* How BuildWise supports practical Software Engineering project development.

The user can then choose to:

* Create an account.
* Log in to an existing account.

The detailed content and design of the landing page will be defined later.

---

## 4. Stage 2 — Account Creation / Login

Users must have an account to use the personalized BuildWise project environment.

### New Users

A new user creates an account using basic account information such as:

* Name.
* Email address.
* Password.
* Other authentication information required by the selected authentication method.

After creating the account, the user proceeds to onboarding.

### Existing Users

Existing users can log in and access their projects and workspace.

Account authentication and security requirements will be defined later during Requirements Engineering.

---

## 5. Stage 3 — Onboarding

After creating an account, BuildWise introduces the user to the platform and collects initial information needed to understand the user's context.

The onboarding process may ask questions such as:

* What best describes the user's current context?
* Is the user a student, recent graduate, trainee, or independent learner?
* Does the user already have a project idea?
* What is the purpose of the project?
* Is the user working individually or with a team?
* What type or domain of project is being considered?
* Is the user associated with a university, training organization, or other institution?

Not all questions are required for every user.

The purpose of onboarding is not to collect information for its own sake, but to provide BuildWise with enough context to personalize the initial project setup and guidance.

---

## 6. Stage 4 — Project Idea

BuildWise supports users who either already have a project idea or do not yet have one.

### 6.1 User Has an Idea

If the user already has an idea, BuildWise helps the user describe and clarify the project context.

This may include understanding:

* The problem being addressed.
* The intended users.
* The general project goal.
* The expected type or domain of the system.

### 6.2 User Does Not Have an Idea

If the user does not have a project idea, BuildWise may help the user explore and develop a suitable project idea.

Possible future approaches may include:

* Guided questions.
* Project idea exploration.
* Example project categories.
* Challenges or project prompts.
* AI-assisted idea generation.

The exact approach is not defined at this stage and will be evaluated during MVP definition.

---

## 7. Stage 5 — Project Setup

Once a project idea or project direction has been established, the user creates or configures a BuildWise project.

The setup may include:

* Project name.
* Project description.
* Project context.
* Project type or domain.
* Project objective.
* Working mode.

### Working Mode

The user may work:

**Solo**

or

**As a Team**

---

## 8. Stage 6 — Team Setup

If the user chooses to work as a team, the user who creates the team/project initially becomes the Team Leader.

The Team Leader may invite other users to join the project.

A simplified team flow is:

**Create Team / Project → Team Leader → Invite Members → Members Accept Invitation → Shared Project Workspace**

All accepted members become associated with the relevant project and can collaborate according to their assigned permissions.

Detailed team roles, permissions, invitations, member management, and leadership rules will be defined later during Requirements Engineering.

---

## 9. Stage 7 — Project Approach

After understanding the project context, BuildWise may help the user identify an appropriate Software Engineering approach for the project.

The guidance may consider factors such as:

* Project characteristics.
* Project size.
* Team or solo context.
* Project goals.
* Expected development process.

BuildWise may suggest possible approaches or methodologies rather than automatically imposing one.

The user remains responsible for understanding and making the final engineering decision.

Detailed methodology support will be defined later.

---

## 10. Stage 8 — Project Workspace

After project setup, the user enters the main BuildWise project workspace.

The workspace becomes the central environment for managing the project's Software Engineering journey.

At a high level, it may provide access to:

* Current project stage.
* Project progress.
* Project activities.
* Project artifacts.
* Team information.
* Project documentation.
* Guidance and recommendations.

The exact workspace structure and features will be defined during MVP and Requirements Engineering.

---

## 11. Stage 9 — Software Engineering Journey

The core BuildWise experience is the structured Software Engineering journey.

A project may progress through activities such as:

**Planning → Requirements → Analysis → Design → Development → Testing → Deployment → Maintenance**

BuildWise should help users understand:

* What they are currently working on.
* Why the activity is needed.
* What should be produced.
* How the current activity connects to previous work.
* What should happen next.

The journey is not necessarily strictly linear.

Users may need to revisit previous activities when new information, requirements, or feedback are discovered.

For example:

**Testing → Feedback → Requirements Update → Design Update → Development → Testing**

This supports the iterative nature of Software Engineering.

---

## 12. Stage 10 — Project Completion

A project reaches a completion state when the user has completed the relevant project activities and produced the expected project outputs.

Completion should not be defined only by whether the software runs successfully.

A completed BuildWise project may include evidence such as:

* Requirements.
* Analysis artifacts.
* Design artifacts.
* Documentation.
* Source code.
* Tests.
* Deployment information.
* Project decisions and history.

The exact completion criteria will be defined later.

---

## 13. Stage 11 — Project Evidence and Optional Sharing

After completing a project, BuildWise may provide users with an organized representation of their project work and Software Engineering experience.

Users may potentially choose how their project is shared:

### Private

The project remains visible only to the user and authorized team members.

### Shared / Unlisted

The user may share the project through a controlled link or similar mechanism.

### Public

The user may choose to make selected project information publicly visible.

A future public project showcase may allow BuildWise to present completed projects and demonstrate practical Software Engineering activity.

Public sharing is optional and should not be required to complete a project.

---

## 14. Platform and User Context Information

During onboarding and project usage, BuildWise may collect relevant contextual information that helps personalize the experience and understand how the platform is being used.

Potential information may include:

* User context.
* Field of study or professional field.
* University or educational institution.
* Training organization.
* Project type.
* Solo or team status.
* Project completion status.

This information may support future product analytics and platform reporting, such as:

* Number of registered users.
* Number of projects created.
* Number of completed projects.
* Distribution of users by context.
* Distribution of projects by type.
* Representation of universities or organizations.

Any collection, storage, visibility, and use of user information will be subject to appropriate privacy and data-management requirements.

These analytics capabilities are not defined as detailed MVP features at this stage.

---

## 15. High-Level Journey Summary

The BuildWise journey can be summarized as:

**1. Discover BuildWise**
↓
**2. Create an account / Log in**
↓
**3. Complete onboarding**
↓
**4. Define or explore a project idea**
↓
**5. Configure the project**
↓
**6. Choose Solo or Team**
↓
**7. Create team and invite members if needed**
↓
**8. Understand the project approach**
↓
**9. Enter the project workspace**
↓
**10. Follow the Software Engineering journey**
↓
**11. Iterate and refine when necessary**
↓
**12. Complete the project**
↓
**13. Preserve project evidence**
↓
**14. Optionally share the project**

---

## 16. Relationship to the MVP

This document describes the desired high-level product journey and does not mean that every stage will be fully implemented in the first BuildWise release.

The next step is to define the **MVP Scope** and determine:

* Which parts of this journey are essential for the first usable version.
* Which capabilities can be simplified.
* Which capabilities should remain outside the MVP.
* Which future ideas should be recorded for later development.

The MVP should preserve the core BuildWise value while keeping the first version focused and achievable.

---

## 17. Discovery Status

**Version:** 0.1

**Status:** Initial high-level user journey hypothesis

This journey represents the current understanding of how users may interact with BuildWise.

It may be refined as MVP scope, requirements, user feedback, and product validation become clearer.
