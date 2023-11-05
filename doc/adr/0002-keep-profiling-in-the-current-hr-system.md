# 2. Keep profiling in the current HR System

Date: 2023-10-17

## Status

Accepted

detailed by [4. decouple HR++](0004-decouple-hr.md)

## Context

The HR people are put up with the task to update profile information of student. Which is cumbersome and error prone. The system has an API

## Decision

We use the HR++ Api to update the profile.

## Consequences

HR is alleviated from the task to update the profiles.

The API is a SOAP api. Hence. Synchronous calls. Hence it only works if the HR++ system is UP. We may need some decoupling there.


