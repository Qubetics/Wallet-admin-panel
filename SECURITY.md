# Security Policy

## Reporting a vulnerability

Please do not open a public issue for security problems.

Email **SECURITY_CONTACT_EMAIL** with:

- a description of the issue and its impact
- steps to reproduce, or a proof of concept
- the affected version or commit

We aim to acknowledge reports within 3 business days and to share a
remediation plan within 14 days. Please give us a reasonable time to fix the
issue before disclosing it publicly.

## Scope

This repository is the Qubetics admin dashboard front end. Reports about the
deployed backend API, the wallet extension, or third-party packages should go to
the respective project, unless the issue is in how this repository uses them.

## Handling secrets

- Never commit `.env` files. `.env.example` lists variable names only.
- Every `REACT_APP_*` value is embedded in the public JavaScript bundle at
  build time and is readable by anyone who loads the site. Do not put
  server-side secrets in them.
- If you find a credential in this repository or its history, report it
  privately so it can be revoked.
