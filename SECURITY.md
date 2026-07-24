# Security Policy

## Supported versions

Security fixes are applied to the latest code on `main` and, when release
branches exist, the latest maintained release. Older commits, forks, and
self-hosted deployments are not separately supported.

## Report a vulnerability

Report suspected vulnerabilities privately through GitHub Security Advisories:

https://github.com/laigit-dot/profile-shop/security/advisories/new

Do not open a public issue, discussion, or pull request for an undisclosed
vulnerability. Include the affected endpoint or component, reproduction steps,
impact, and any suggested mitigation. Avoid accessing data that is not yours,
disrupting services, or performing destructive testing.

The maintainer aims to acknowledge a report within 7 days and provide a status
update within 14 days. These are targets, not guarantees; availability,
complexity, and the need to coordinate disclosure can affect timing. Reporters
will be kept informed when practical, and public disclosure will be coordinated
after a fix or mitigation is available.

## Secrets and deployment safety

- Never commit `.env`, GitHub tokens, Giphy API keys, or other credentials.
- Use least-privilege credentials and separate development and production
  keys.
- If a credential is exposed, revoke or rotate it through the relevant
  provider and remove it from active deployments. Deleting it from the latest
  commit alone does not remove it from Git history.
- Review logs, caches, and generated SVG responses before exposing them
  publicly.

Self-hosters are responsible for deployment security, access controls,
monitoring, updates, and provider usage. GitHub and Giphy apply their own API
terms, quotas, and rate limits. A public deployment can exhaust those quotas or
incur provider restrictions, especially if it allows unrestricted requests.
Use caching, request limits, scoped credentials, and provider dashboards
appropriate to your deployment.
