# 4. decouple HR++

Date: 2023-11-05

## Status

Accepted

details [2. Keep profiling in the current HR System](0002-keep-profiling-in-the-current-hr-system.md)

detailed by [9. use events for communicating between components](0009-use-events-for-communicating-between-components.md)

## Context

The HR++ system has a SOAP API. Which is synchoronous. We cannot guarentee that the system is always up. It has a history of flakeyness. We also need to keep the portfolio update guarenteed.

## Decision

Decouple portfolio updates in time by deploying a separate component that manages the coupling. It caches the portfolio updates and guarentees delivering it to HR++

## Consequences

We need to deploy a separate component, which complicates the deployment architecture a bit. 
