# Maintaining Fitlyn Public Documentation

This repository contains only customer-safe documentation.

## Update workflow

1. Product behavior changes in the private application repository.
2. Update the complete internal documentation in that implementation PR.
3. Decide whether the change is useful and safe for customers.
4. If public documentation is affected, open a separate PR here.
5. Have the other teammate review the content and safety checklist.
6. Merge to publish automatically through GitHub Pages.

## Allowed content

- User-facing product explanations
- Setup and daily-operation guides
- Screenshots containing test data only
- General troubleshooting steps
- Public release notes

## Prohibited content

- Source code or private repository links
- Database schemas, migrations, RLS policies, or internal architecture
- Security findings, exploit details, incidents, or audit reports
- API keys, tokens, credentials, internal URLs, or environment values
- Customer names, phone numbers, payment data, exports, or production screenshots
- Internal deployment, rollback, provider, or administrative procedures

## Review requirements

- Confirm statements match current production behavior.
- Remove implementation details that do not help users.
- Use test data in examples and screenshots.
- Check every link.
- Build with `mkdocs build --strict`.

