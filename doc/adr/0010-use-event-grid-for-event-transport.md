# 10. use event grid for event transport

Date: 2023-11-14

## Status

Accepted

## Context

We want event based communication to be asynchronous and based on azure cloud native services. We do not want to maintain our own kafka installation.

## Decision

We use event grid for event transport

## Consequences

This is locking in azure a bit more, but with the use of heaxonal architecture we can reduce that to some extent.
