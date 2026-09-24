# Constraints and Assumptions

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1
**Status:** Draft

## 1. Purpose

This document defines the main constraints and assumptions that currently affect the design and development of the BuildWise MVP.

These may be refined as the product is validated and more implementation decisions are made.

---

# 2. Constraints

### CA-01 — MVP Scope

The initial version of BuildWise shall focus on helping Software Engineering learners follow a structured project journey and produce connected project work.

Advanced capabilities outside the MVP shall not be required for the initial release.

### CA-02 — No Organizational Features in MVP

The MVP shall not require dedicated functionality for universities, training organizations, instructors, supervisors, mentors, or evaluators.

These stakeholders are part of the future direction of BuildWise.

### CA-03 — No Advanced Collaboration in MVP

The MVP shall support basic Solo and Team projects but shall not require advanced real-time collaboration, complex permissions, or real-time document editing.

### CA-04 — No GitHub or IDE Integration in MVP

The MVP shall not depend on GitHub, external repositories, or an integrated development environment.

Source code may remain outside BuildWise, with relevant references or evidence recorded in the project when applicable.

### CA-05 — No Advanced AI Dependency

The core BuildWise MVP shall not depend on advanced AI features.

AI-assisted guidance, artifact review, code assistance, and similar capabilities may be introduced in future versions.

### CA-06 — Web-Based Product

BuildWise is initially defined as a web-based application.

The MVP shall therefore be designed for use through modern web browsers.

### CA-07 — Evolving Requirements

BuildWise is being developed iteratively using an Agile approach.

Requirements may change as the product is developed and validated.

---

# 3. Assumptions

### CA-08 — Basic Software Engineering Knowledge

The primary target users are assumed to have at least some academic or practical exposure to Software Engineering and programming concepts.

BuildWise provides guidance and context but is not intended to replace foundational Software Engineering education.

### CA-09 — User Has or Can Define a Project

A User may enter BuildWise with an existing project idea or without one.

The system should support both situations within the MVP scope.

### CA-10 — Project Work May Be Solo or Team-Based

A User may work individually or as part of a team.

The working mode is defined at the project level.

### CA-11 — Users Contribute Project Work

BuildWise assumes that users will actively create, review, and update their own project artifacts and activities.

The platform guides the process but does not automatically complete the project for the user.

### CA-12 — Project Artifacts May Be External

Not all project outputs need to be created or stored entirely inside BuildWise.

Some outputs, such as source code or externally created documents, may remain outside the platform while relevant references or evidence are maintained in BuildWise.

### CA-13 — Project Privacy by Default

Project information shall be private by default within BuildWise. Public project discovery and showcase features are outside the MVP scope. Users may still share their project through external platforms or services.

Public project sharing is outside the MVP scope.

### CA-14 — Initial Usage Scale Is Not Yet Defined

The expected number of users, projects, and concurrent sessions has not yet been established.

Specific infrastructure and scalability targets will therefore be defined later based on deployment and validation needs.

---

# 4. Future Refinement

These constraints and assumptions may be updated when:

* User validation provides new evidence
* MVP implementation reveals new limitations
* Architecture decisions are made
* Deployment requirements become clearer
* New BuildWise capabilities are introduced

Changes to these assumptions may require related requirements and design decisions to be reviewed.
