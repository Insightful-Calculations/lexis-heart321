# Security Policy

## Reporting vulnerabilities

If you discover a security vulnerability in any code or system associated with this project, please report it responsibly:

1. **Do NOT open a public issue**
2. Email: [PLACEHOLDER_EMAIL]
3. Include: description, reproduction steps, potential impact

We aim to acknowledge reports within 48 hours.

## Scope

This repository contains research publications and data. The computational research system operates in a separate, private environment with its own security architecture.

## Automated systems

Currently, no automated agents process public input from this repository. All issues, PRs, and comments are human-reviewed only.

If automated processing is enabled in the future, all external inputs will be processed through input validation and prompt injection detection before reaching any automated agent. Suspicious activity will trigger incident reporting.

## Threat model

We are aware that public-facing AI agent systems create attack surfaces including prompt injection, poisoned contributions, and social engineering. The security architecture follows a fractal defense-in-depth model. Details will be published when the public automation layer is active.

## Supported versions

| Version | Supported |
|---------|-----------|
| v62     | Yes       |
| < v62   | Not applicable (v62 is the first public release) |
