# Contributing to YouthMind

Thank you for helping improve YouthMind. Product repositories may be private,
but the same engineering expectations apply across the organization.

## Before you start

1. Reference an issue that states the user problem and acceptance criteria.
2. Keep the change narrowly scoped; avoid unrelated formatting or generated files.
3. Never commit credentials, production data, private health information, signing
   material, or screenshots containing identifiable user content.
4. Treat authentication, safety, privacy, deletion, moderation, recommendation,
   and AI behavior changes as high risk and add explicit tests.

## Pull requests

- Explain the problem, approach, risks, and rollback path.
- Include tests for observable behavior and contract changes.
- Attach before/after evidence for UI, latency, reliability, or quality claims.
- Identify migrations, environment variables, external services, and operational steps.
- Run the affected test suites, `git diff --check`, and a secret scan.
- Do not describe a local smoke test as production validation.

## Commit hygiene

Use focused, imperative commit messages. Keep build products, logs, local IDE
state, `.env` files, datasets, and test credentials out of version control.

## Responsible product language

YouthMind is a general-wellbeing product. Do not add diagnostic, treatment, or
emergency-service claims without the required legal, clinical, and regulatory review.
