# 5. Running and enrolling are deployed together

Date: 2023-11-05

## Status

Accepted

Detailed by [6 Append only store for attendance](0006-append-only-store-for-attendenace.md)

## Context

Since most trainings courses start at 9, we will have busy times in registering training attendance at the beinning of the training. With the current forecasted number of training courses, teachers and clients we feel that we can cope.

Running and enrolling seem to be quite related. It is all about one training course (instance).

## Decision

We deploy enrolling and running as separate modules in one physical component.

## Consequences

It simplifies the deployment. There is a slight risk that monday mornings are somewhat busy with presence registrations.
