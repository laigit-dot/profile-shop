# Releasing GitHub Deco

GitHub Deco uses Semantic Versioning and GitHub Releases. It is a private npm
package (`"private": true`) and is not published to npm.

## Prepare a release

1. Start from a reviewed, passing `main` branch.
2. Confirm merged pull requests have clear titles and were squash merged,
   except Dependabot updates, which use merge commits so the following CodeQL
   run retains write access to security events.
3. Choose the next version according to
   [Semantic Versioning](https://semver.org/):
   - patch for backward-compatible fixes
   - minor for backward-compatible features
   - major for incompatible API or behavior changes
4. Run the complete quality suite:

   ```sh
   npm ci
   npm run lint
   npm run typecheck
   npm test
   npm run build
   ```

5. Update the package version and prepare release notes from the changes since
   the previous release. The notes serve as the project changelog and should
   call out breaking changes, migrations, security fixes, and contributor
   credits.
6. Submit release preparation through the normal pull request review process.

## Publish on GitHub

After the release pull request is merged:

1. Create a `vX.Y.Z` tag from the reviewed commit on `main`.
2. Create a GitHub Release for that tag.
3. Use the prepared changelog as the release notes and verify links and
   examples before publishing.
4. If a release must be corrected, make the correction through a new reviewed
   commit and version rather than moving an already published tag.

Do not run `npm publish`, add package-registry credentials, or place npm tokens
in repository or release configuration.
