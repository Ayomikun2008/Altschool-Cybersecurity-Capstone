# Internal Employee Portal Security Audit

## Overview

This project involved a security assessment of an internal employee portal, focusing on authorization and access-control weaknesses.

## Objective

The objective was to determine whether an authenticated employee could access resources belonging to another user by manipulating object identifiers in application requests.

## Vulnerability Tested

- Insecure Direct Object Reference (IDOR)
- Broken Access Control
- Improper Authorization

## Tools Used

- Burp Suite
- Web Browser
- HTTP Requests

## Methodology

1. Authenticated to the application using a test account.
2. Identified requests containing object or user identifiers.
3. Intercepted requests using Burp Suite.
4. Modified the relevant identifier.
5. Replayed the modified request.
6. Observed whether unauthorized resources could be accessed.
7. Documented the security impact and recommended remediation.

## Security Impact

An IDOR vulnerability can allow an authenticated user to access information or functionality belonging to another user without proper authorization.

## Recommendation

Implement server-side authorization checks for every requested object and verify that the authenticated user has permission to access the requested resource.

## Evidence

Screenshots and supporting documentation will be added to this directory.
