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

After creating the account, the user may proceed to onboarding.

### Existing Users

Existing users can log in and access their projects and workspace.

### Users Invited to a Team

A user does not necessarily need to have an existing BuildWise account before receiving a team invitation.

If a Team Leader invites someone who does not yet have an account, the invited user can:

**Open Invitation → Sign Up → Accept Invitation → Join the Team Project**

If the invited user already has an account, the flow can be:

**Open Invitation → Log In → Accept Invitation → Join the Team Project**

This allows team invitations to serve as an entry point to BuildWise for new users.

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

If the user enters BuildWise through a team invitation, the system already knows that the user is joining a specific team/project. Therefore, the user does not need to independently choose between Solo and Team for that project.

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

The project may be worked on:

**Solo**

or

**As a Team**

The working mode describes how the user is working on a specific project. It is not a permanent attribute of the user's account.

A user may work on one project individually, while being a Team Leader or Team Member on another project.

---

## 8. Stage 6 — Team Setup

If the user chooses to work as a team, the user who creates the team/project initially becomes the Team Leader.

The Team Leader may invite other users to join the project.

A simplified team flow is:

**Create Team / Project → Team Leader → Send Invitation → Member Opens Invitation → Log In or Sign Up → Accept Invitation → Join Shared Project Workspace**

A user who receives an invitation does not need to independently select "Team" for that project because the invitation already identifies the relevant team/project.

Once the invitation is accepted, the user's account becomes associated with the relevant team/project as a member.

All accepted members can collaborate according to their assigned permissions.

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

During account creation, onboarding, and project usage, BuildWise may collect relevant contextual information that helps personalize the experience and understand how the platform is being used.

### User Profile Information

Information about the person should be associated with the user's account/profile, such as:

* User context.
* Field of study or professional field.
* University or educational institution.
* Training organization.
* Other relevant background information.

These attributes describe the user and should not depend on whether the user enters BuildWise directly or through a team invitation.

### Project Information

Information about a specific project may include:

* Project type.
* Project domain.
* Solo or team status.
* Project completion status.

This distinction allows one user to participate in different projects with different working modes.

### Platform Analytics

Aggregated information may support future product analytics and platform reporting, such as:

* Number of registered users.
* Number of projects created.
* Number of completed projects.
* Distribution of users by context.
* Distribution of users by field of study or professional field.
* Representation of universities or organizations.
* Distribution of projects by type.
* Distribution of solo and team projects.

Any collection, storage, visibility, and use of user information will be subject to appropriate privacy and data-management requirements.

These analytics capabilities are not defined as detailed MVP features at this stage.

---

## 15. High-Level Journey Summary

The BuildWise journey can be summarized as:

**1. Discover BuildWise**<br>
↓<br>
**2. Create an account / Log in**<br>
↓<br>
**3. Complete onboarding**<br>
↓<br>
**4. Define or explore a project idea**<br>
↓<br>
**5. Configure the project**<br>
↓<br>
**6. Choose Solo or Team**<br>
↓<br>
**7. Create team and invite members if needed**<br>
↓<br>
**8. Understand the project approach**<br>
↓<br>
**9. Enter the project workspace**<br>
↓<br>
**10. Follow the Software Engineering journey**<br>
↓<br>
**11. Iterate and refine when necessary**<br>
↓<br>
**12. Complete the project**<br>
↓<br>
**13. Preserve project evidence**<br>
↓<br>
**14. Optionally share the project**

For users entering through a team invitation, the relevant path may instead be:

**Invitation → Sign Up / Log In → Accept Invitation → Team Project Workspace**

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

**Version:** 0.2

**Status:** Refined high-level user journey hypothesis

This journey represents the current understanding of how users may interact with BuildWise.

It may be refined as MVP scope, requirements, user feedback, and product validation become clearer.
