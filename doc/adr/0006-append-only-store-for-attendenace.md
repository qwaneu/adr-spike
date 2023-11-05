# 6. Append only store for attendenace

Date: 2023-11-05

## Status

Accepted

details [5 Running and enrolling are deployed together](0005-running-and-enrolling-are-deployed-together.md)

## Context

It can be busy on mondays while registering attendance of all trainings. We decided to keep enrolling and running together in one componnet.

## Decision

We use an appennd only store for registering attendance. 

## Consequences

Registering attendence does not require big locks around big relational models, making us prepared on growth.


