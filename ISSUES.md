# Prepared GitHub Issues for skills-integrate-mcp-with-copilot

Below are prepared issues for features inspired by the `andreabac3/dsc-website-template` comparison. Create them as real GitHub issues from this file or ask me to create them directly (I can open issues if you grant me repo access/token).

---

## 1) Add Gatsby static site (React + GraphQL) and build system
**Description:** Introduce a Gatsby-based static site in a new `web/` directory to replace or complement the current `src/static` frontend. Add Node project files (`package.json`) and scripts for `develop`, `build`, and `deploy`.

**Acceptance criteria:**
- `web/` contains a working Gatsby starter site that builds successfully with `npm run build`.
- `package.json` includes `develop`, `build`, `deploy` scripts.
- README updated with quickstart for the Gatsby site.

**Labels:** enhancement, frontend, gatsby

---

## 2) Add content-driven YAML `content/` folder and content schema
**Description:** Add a `web/content/` folder containing YAML files (e.g., `teams.yaml`, `opportunities.yaml`, `faqs.yaml`) to make the site editable by non-developers.

**Acceptance criteria:**
- `web/content/` has example YAML files for teams, overview, opportunities, technologies, and footer.
- README documents how to edit content files to update the site.

**Labels:** enhancement, content

---

## 3) Integrate `gatsby-transformer-yaml` + GraphQL data pipeline
**Description:** Configure `gatsby-source-filesystem` and `gatsby-transformer-yaml` so content YAML is available via GraphQL to React components.

**Acceptance criteria:**
- Gatsby `gatsby-config.js` includes configured plugins.
- Example GraphQL query in a page/component demonstrates reading `teams` or `opportunities`.

**Labels:** enhancement, gatsby

---

## 4) Replace static frontend with modular React components
**Description:** Implement modular React components for `Overview`, `Teams`, `Opportunities`, `Workshops`, `Faqs`, and `Technologies` under `web/src/components/` and use GraphQL queries to populate them.

**Acceptance criteria:**
- Each component exists and renders content from the YAML files.
- The homepage composes these components and matches current information.

**Labels:** enhancement, frontend

---

## 5) Add SASS + Bootstrap (`react-bootstrap`) styling and `Layout.scss`
**Description:** Add `gatsby-plugin-sass`, Bootstrap and `react-bootstrap` to the frontend; create a shared `Layout.scss` and responsive layout components.

**Acceptance criteria:**
- Styling is implemented with SASS files and Bootstrap is available for components.
- The site is responsive at common breakpoints.

**Labels:** enhancement, styling

---

## 6) Add FontAwesome icons integration and `src/icons.js`
**Description:** Add FontAwesome packages and an `icons.js` module to centralize icon imports for components (teams, footer, social links).

**Acceptance criteria:**
- FontAwesome packages are in `web/package.json` and `web/src/icons.js` exports the icons used by components.
- README explains how to add new social icons.

**Labels:** enhancement, ui

---

## 7) Add image optimization (`gatsby-image`, `sharp`) and SEO component
**Description:** Include `gatsby-image`, `gatsby-plugin-sharp`, and `gatsby-transformer-sharp` to optimize images; add `src/components/seo.js` to manage page metadata.

**Acceptance criteria:**
- Images in `content/` or `src/images/` are processed and used via `gatsby-image`.
- An `seo.js` component exists and sets title/meta tags for pages.

**Labels:** enhancement, performance, seo

---

## 8) Add PWA/offline support and deployment scripts (`gh-pages`, Firebase)
**Description:** Add `gatsby-plugin-manifest` and `gatsby-plugin-offline` for PWA/offline support. Add deploy scripts to `package.json` for GitHub Pages (`gh-pages`) and an optional `deployFirebase` script with instructions.

**Acceptance criteria:**
- `web/package.json` contains `deploy` and (optional) `deployFirebase` scripts.
- Manifest and offline plugins are configured; site works offline after build.
- README explains deploy steps for GitHub Pages and Firebase.

**Labels:** enhancement, infra, pwa

---

If you want me to create these as actual GitHub issues, give me permission to create issues in the repository (or provide a token), and I will open them for you.