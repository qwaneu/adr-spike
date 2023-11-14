# 9. use events for communicating between components

Date: 2023-11-14

## Status

Accepted

details [8. separate deployment of course development from runnning and enrolling](0008-separate-course-development-from-runnning-and-enrolling.md)

details [4. decouple HR++](0004-decouple-hr.md)

detailed by [10. use event grid for event transport](0010-use-event-grid-for-event-transport.md)

## Context

We decided to decouple HR++ and to have separate deployments of some components (notably course development separated from running and enrolling). These separate deployments are not effective when they are coupled by point to point synchronous communication. They would depend on each others presence then. Moreover, the status updates in the communication between these components eventually consistent.

## Decision

We use event based communication between separatly deployed components.

## Consequences

Deployment of components becomes easier as they are not dependent on each others uptime. It is a bit harder to reason about the flow of control in updates between components.
