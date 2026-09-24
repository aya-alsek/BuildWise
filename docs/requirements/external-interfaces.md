# External Interfaces

**Product:** BuildWise
**Phase:** Requirements Engineering
**Version:** 0.1
**Status:** Draft

## 1. Purpose

This document identifies the external interfaces through which BuildWise interacts with users, external software services, or communication mechanisms.

It defines the required external interactions at a requirements level without specifying implementation technologies or service providers.

## 2. User Interface

BuildWise shall provide a web-based user interface through which users can:

* Create and access their accounts
* Configure and manage projects
* Work through the Software Engineering journey
* Create and manage project artifacts
* Track project progress
* Review project evidence and completion information
* Participate in Team Projects according to their project permissions

The interface shall support the usability and accessibility requirements defined in the Non-Functional Requirements.

## 3. Email Interface

BuildWise may require an email service to support functions such as:

* Account recovery
* Project invitations
* Other account-related or project-related notifications where required

The specific email service and technical communication mechanism will be determined during Design and Implementation.

## 4. Source Code and External Project References

Users may provide references to external project resources, such as source-code repositories or deployed project environments, as part of their project evidence.

For the MVP, these references may be stored as user-provided links.

Direct integration with external development platforms such as GitHub is outside the current MVP scope.

## 5. Future External Interfaces

The following interfaces may be considered in future versions of BuildWise:

* GitHub or other source-code platforms for repository integration
* AI services for artifact analysis, guidance, or code-related assistance
* University or academic systems
* Training organization systems
* Mentor or supervisor platforms
* External deployment or hosting services

These interfaces are not required for the current MVP.

## 6. Security of External Communication

External communication involving user or project information shall use appropriate security mechanisms.

Sensitive information shall not be transmitted through unsecured communication channels.

Detailed communication protocols, authentication mechanisms, and integration security requirements will be defined during Design and Implementation.

## 7. Interface Scope

The current MVP focuses on the core BuildWise experience and minimizes dependency on external systems.

The MVP shall therefore:

* Provide the main functionality through the BuildWise web interface
* Use external email communication where required
* Allow users to include manually provided external references as part of project evidence, without requiring direct integration with external platforms.
* Avoid requiring direct integration with external development, AI, academic, or organizational platforms

External integrations may be introduced incrementally in future iterations as validated product needs emerge.

## 8. Relationship to Later Design

This document defines **what external interactions BuildWise may require**, not how those interactions will be implemented.

Detailed interface specifications, APIs, communication protocols, authentication mechanisms, and integration architecture will be defined during later Design and Implementation activities.
