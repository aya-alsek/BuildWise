# Business Rules

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1

## 1. Purpose

This document defines the business rules that govern how BuildWise projects, users, teams, activities, and project work are handled.

These rules describe constraints and conditions that the system must follow regardless of the implementation technology.

---

## 2. User and Account Rules

### BR-01 — Single Account Type

BuildWise shall use a single authenticated account type: **User**.

Student, Recent Graduate, Trainee, and Independent Learner are user contexts and shall not create separate account roles.

### BR-02 — User Context

A User may have a context such as Student, Recent Graduate, Trainee, or Independent Learner.

The context may be used to support onboarding and relevant guidance but shall not determine project permissions by itself.

### BR-03 — Account Ownership

Each BuildWise account belongs to one User.

---

## 3. Project Rules

### BR-04 — Project Ownership

Each project shall have exactly one Project Owner.

### BR-05 — Multiple Projects

A User may participate in multiple projects.

A User's role may differ between projects.

### BR-06 — Working Mode

Each project shall have one working mode:

* Solo
* Team

### BR-07 — Solo Project

A Solo Project has one Project Owner and does not require team members.

### BR-08 — Team Project

A Team Project has a Project Owner and may include one or more Team Members.

### BR-09 — Team Leader

For a Team Project, the Project Owner is the Team Leader.

Team Leader is not a separate account role.

---

## 4. Team Membership Rules

### BR-10 — Team Membership

A User becomes a Team Member only after accepting an invitation to a Team Project.

### BR-11 — Invitation

A project invitation shall be associated with a specific project and invited person.

### BR-12 — Project Access

A User may access private project information only when they are the Project Owner or an authorized Team Member of that project.

### BR-13 — Project Role Scope

Project roles apply only within the project to which they are assigned.

A User being a Project Owner in one project does not give them Owner permissions in another project.

---

## 5. Software Engineering Journey Rules

### BR-14 — Project Journey

Each project shall follow the BuildWise Software Engineering journey defined for the applicable project type and MVP scope.

The MVP journey consists of:

1. Project Understanding
2. Requirements
3. Analysis
4. Design
5. Implementation
6. Testing
7. Completion

### BR-15 — Stage Progress

Project progress shall be based on the completion of relevant activities and outputs within the applicable stages.

### BR-16 — Iterative Work

Users may revisit and update previously completed project work.

Completing a stage does not permanently prevent changes to earlier work.

---

## 6. Artifact Rules

### BR-17 — Project Association

Each project artifact shall belong to a specific project.

### BR-18 — Artifact Context

Artifacts shall be associated with the relevant Software Engineering stage or activity when applicable.

### BR-19 — Authorized Modification

Only project participants with the required permissions may create or modify project artifacts.

### BR-20 — Artifact Updates

Updating an artifact shall not remove its association with the project or its relevant engineering context.

---

## 7. Project Completion Rules

### BR-21 — Completion Readiness

A project shall only be considered ready for completion when its required MVP activities and outputs have been completed.

### BR-22 — Project Completion

The Project Owner is responsible for marking the project as completed.

### BR-23 — Completion and Previous Work

A completed project may retain its artifacts and evidence for review.

Future changes to completed projects may be subject to additional rules defined in later versions.

---

## 8. Privacy Rules

### BR-24 — Private Project Data

Project data shall be private by default.

### BR-25 — Authorized Access

Private project data shall only be accessible to users who have the required project permissions.

### BR-26 — User Context and Privacy

A user's context shall not grant access to another user's project or project data.

---

## 9. MVP Rule Scope

The rules in this document apply to the BuildWise MVP.

Advanced rules related to:

* Detailed team permissions
* Mentors and supervisors
* Universities and training organizations
* Public project portfolios
* Advanced collaboration
* GitHub integration
* AI-assisted project review

are outside the current MVP and will be defined when the corresponding features are introduced.
