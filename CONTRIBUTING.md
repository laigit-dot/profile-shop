# Contributing to GitHub Deco

Thanks for helping improve GitHub Deco.

## Before you start

- Use Node.js 22.12 or newer. The repository includes `.nvmrc` for the current
  Node.js 24 LTS release.
- For substantial features, API changes, or broad refactors, open an issue
  before writing code so the scope can be agreed on.
- Use a focused branch name such as `feat/card-layout`, `fix/giphy-timeout`,
  `docs/self-hosting`, or `chore/dependencies`.
- Never commit `.env`, access tokens, API keys, or other credentials. Use only
  personal development keys with the minimum permissions needed.

## Local setup

```sh
npm ci
cp .env.example .env
npm run dev
```

Fill in `.env` with your own GitHub and Giphy credentials. Do not share keys or
reuse production credentials for local development.

## Quality checks

Run every check before submitting a pull request:

```sh
npm run lint
npm run typecheck
npm test
npm run build
```

Add or update tests when behavior changes. Keep documentation and examples in
sync with public API changes.

## Pull requests

1. Fork the repository and create a branch from the latest `main`.
2. Keep each pull request focused on one coherent change.
3. Explain the motivation, implementation, and verification in the pull
   request description.
4. Link the relevant issue when one exists.
5. Respond to review feedback and keep the branch current enough to merge
   safely.

External pull requests require maintainer review. Maintainers generally squash
merge accepted pull requests.

## Contribution licensing

By submitting a contribution, you agree that it is licensed under the
repository's [MIT License](LICENSE). You must have the right to submit all code,
documentation, and assets included in your contribution and must preserve any
required third-party notices.

GitHub Deco does not currently require a Contributor License Agreement (CLA)
or Developer Certificate of Origin (DCO) sign-off.

Please follow the [Code of Conduct](CODE_OF_CONDUCT.md) in all project spaces.
