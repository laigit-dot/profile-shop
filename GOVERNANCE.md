# Governance

GitHub Deco is currently maintained by
[@laigit-dot](https://github.com/laigit-dot).

## Decision making

Project decisions should be discussed in issues and pull requests whenever
practical. The maintainer seeks consensus by considering technical quality,
user impact, maintainability, security, and alignment with the project's
scope. When consensus cannot be reached in a reasonable time, the current
maintainer makes the final decision and records the rationale publicly.

The maintainer may delegate areas of responsibility to recurring contributors.
Governance changes should be proposed and reviewed like other substantial
project changes.

## Reviews and merging

- External pull requests require maintainer review before merging.
- The author should not treat automated checks as a substitute for review.
- Accepted pull requests are normally squash merged into `main`.
- Dependabot pull requests use a merge commit after checks pass. Preserving a
  maintainer-authored merge commit keeps the following `main` CodeQL run from
  receiving Dependabot's restricted token permissions.
- When the project has at least two active maintainers, changes authored by a
  maintainer will require approval from another maintainer before merging.

## Conflicts of interest

Reviewers should disclose meaningful personal or commercial conflicts and
recuse themselves when those conflicts could affect a decision. The maintainer
may request an independent technical review where practical.

## Emergency changes

A maintainer may bypass the normal review process to address an actively
exploited vulnerability, credential exposure, severe service disruption, or
similarly urgent risk. The bypass should be as narrow as possible. A follow-up
issue or pull request must document the change, verification, and any remaining
work once disclosure is safe.
