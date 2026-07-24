# Third-Party Notices

This file summarizes third-party code and assets directly used by GitHub Deco.
It is informational and does not replace the license files or terms provided
by each upstream project.

## Runtime dependencies and bundled assets

### Hono

- Package: `hono`
- Project: https://hono.dev/
- License reported by the installed package: MIT
- Use: HTTP application and routing framework; bundled into the server build.

### Skill Icons for Iconify

- Package: `@iconify-json/skill-icons`
- Project: https://icon-sets.iconify.design/skill-icons/
- License reported by the installed package: MIT
- Use: the package's Iconify JSON SVG bodies are imported and embedded in
  generated cards and the gallery.

The icons depict third-party products and brands. Their names, logos, and
trademarks remain subject to the rights and usage policies of their respective
owners.

### Simple Icons

- Package: `simple-icons`
- Project: https://simpleicons.org/
- License reported by the installed package: CC0-1.0
- Use: selected brand SVG paths are embedded in contact and donation sections.

Simple Icons' data license does not grant permission to use third-party
trademarks. Deployers and contributors are responsible for following
applicable brand guidelines.

## Remote content and services

GitHub Deco can request data from GitHub and GIF media from Giphy. That
provider-hosted data is not included in this repository and is not
relicensed under the GitHub Deco license. Operators must follow the providers'
current API terms, rate limits, attribution, and branding requirements. In
particular, any Giphy-powered experience should retain the provider branding
and attribution required by Giphy's current terms.

The design reference at
`design/GitHub Profile Card Builder Redesign/GitHub Deco Redesign.dc.html`
loads Inter and Space Grotesk from Google Fonts when opened. Font files are not
stored in this repository; use of that remote service and those fonts remains
subject to their respective terms and licenses.

## Maintainer provenance note

The checked-in `design/GitHub Profile Card Builder Redesign/` reference,
including `support.js`, `.thumbnail`, and the matching archive, predates this
notice. `support.js` identifies itself only as generated from
`dc-runtime/src/*.ts`; the repository does not contain that source, an upstream
URL, or a license notice. The archive and thumbnail likewise do not record
their creation source or authorship. These files are not imported by the
application runtime, and no evidence reviewed here establishes that
redistribution is prohibited, so they have been retained. Before distributing
the design bundle separately or treating it as reusable source, a maintainer
should identify its origin and confirm the applicable license.

For the complete installed dependency graph and package-reported license
identifiers, see `package-lock.json` and the license files shipped in each
installed package.
