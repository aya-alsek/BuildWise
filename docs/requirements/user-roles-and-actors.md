# User Roles and Actors

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1

## 1. Purpose

This document defines the main system actors and project-level roles in BuildWise.

It also distinguishes between a user's **context** and their **role**, so that user characteristics are not confused with system permissions.

---

## 2. User Model

BuildWise uses a single authenticated account type: **User**.

A user's context may be one of the following:

* Student
* Recent Graduate
* Trainee
* Independent Learner

These are **user contexts, not system roles**. They may be used during onboarding to provide relevant guidance, but they do not determine project permissions.

---

## 3. System Actors

### 3.1 Visitor

An unauthenticated person accessing BuildWise.

A Visitor can:

* View the landing page
* Register for an account
* Log in

A Visitor cannot access private user or project data.

### 3.2 User

An authenticated BuildWise account holder.

A User can:

* Manage their account
* Create and access projects
* Participate in projects according to their project role
* Work through the Software Engineering journey
* Create and manage project artifacts
* Track and update project progress

---

## 4. Project Roles

Project roles are assigned per project. The same User may have different roles in different projects.

### 4.1 Project Owner

The Project Owner is responsible for a project.

The Project Owner can:

* Create and configure a project
* Define project information and objectives
* Manage the project
* Invite team members when applicable
* Access and manage project artifacts
* Track project progress
* Complete the project

For a **Solo Project**, the Project Owner works individually.

For a **Team Project**, the Project Owner also acts as the **Team Leader**.

### 4.2 Team Member

A Team Member participates in a Team Project without being the Project Owner.

A Team Member can:

* Accept a project invitation
* Access the shared project workspace
* Participate in project activities
* Contribute to project artifacts
* View project progress
* Perform permitted project work

Detailed team permissions may be expanded in future versions.

---

## 5. Role Relationships

```text
User
│
├── Project Owner
│   └── Team Leader (when the project is a Team Project)
│
└── Team Member
```

The user's context is separate from their project role:

```text
User
├── Context: Student / Graduate / Trainee / Independent Learner
└── Project Role: Project Owner / Team Member
```

A User may be:

* Project Owner of one project
* Team Member of another project
* Project Owner of a Solo project

---

## 6. MVP Scope

### Included

**System Actors**

* Visitor
* User

**Project Roles**

* Project Owner
* Team Member

### Not Separate Roles

The following are not separate system roles in the MVP:

* Student
* Recent Graduate
* Trainee
* Independent Learner
* Team Leader

Student, Graduate, Trainee, and Independent Learner are user contexts, while Team Leader is represented by the Project Owner role for Team Projects.

---

**Status:** Draft — Version 0.1
