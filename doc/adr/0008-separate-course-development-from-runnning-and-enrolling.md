# 8. separate deployment of course development from runnning and enrolling

Date: 2023-11-14

## Status

Accepted

detailed by [7. use container instances for back end components](0007-use-container-instances-for-back-end-components.md)

detailed by [9. use events for communicating between components](0009-use-events-for-communicating-between-components.md)

## Context

Availability and performance characteristics if running and enrolling training courses are very different from course development. We foresee scaling to be necessary in running and enrolling way sooner than in course development.

## Decision

We separate deployment of running and enrolling from course development.

## Consequences

It will be easier to reason about scaling running and enrolling. The development of course development can be done in a separate team. The communication between components need some extra though though.
