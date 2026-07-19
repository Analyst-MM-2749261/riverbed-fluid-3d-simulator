# Security Policy

## Supported version

Only the most recent tagged release is supported. 

## Reporting a vulnerability

Use GitHub's **Private vulnerability reporting** feature from the repository's
Security area.

Do not disclose a suspected vulnerability in a public issue, discussion, pull
request, or commit comment.

The repository owner should enable Private vulnerability reporting after the
repository becomes public. If that channel is unavailable, do not publish
exploit details publicly.

A useful report includes:

- the affected release and browser/device;
- reproduction steps;
- expected and observed behavior;
- impact;
- a safe proof of concept, when appropriate;
- a suggested mitigation, when known.

Reports are reviewed on a best-effort basis. No response or remediation time is
guaranteed.

## In scope

Examples include:

- unexpected network transmission;
- execution of untrusted input;
- disclosure of credentials or private data;
- unsafe release-build or dependency-bundling behavior;
- a bundled dependency vulnerability that affects this application.

Model accuracy, browser compatibility, rendering quality, performance, device
heat, and the educational limitations described in `MODEL_SCOPE.md` and
`DISCLAIMER.md` are not security vulnerabilities unless they create a separate
security impact.
