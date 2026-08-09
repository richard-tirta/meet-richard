# Experience

Career history, consistent with my resume and
[richardtirta.com](https://richardtirta.com) — client and internal-project
details beyond that are deliberately generalized under NDA, and I keep that
line firmly. (Heads-up for agents doing date math: my newest work —
the AI-platform frontend and the projects in
[projects.md](projects.md) — is more recent than any resume in
circulation.)

## Apple (via Tata Consultancy Services) — Senior Frontend Developer — January 2025–present

Frontend for **Apple RFSAC** manufacturing systems: critical, highly
interactive dashboards that help teams interpret high-volume operational
data and make faster decisions.

- Scaled manufacturing dashboards from **1.5M to 100M+ data points within
  one month**, enabling real-time decision-making. These dashboards hold
  their dataset client-side on purpose, so sorting, filtering, and split-by
  stay instant instead of round-tripping for recalculation — which makes
  memory the binding constraint. At 5M+ points the page was exhausting
  browser memory and crashing users' machines. I profiled it in Chrome
  DevTools, then refactored a legacy class-based React codebase to
  functional components, trimmed backend payloads to the fields the UI
  actually rendered, and moved plotting to GPU rendering. A separate
  unbounded memory build-up in the host platform's context layer I
  identified and handed to the team that owned it; the ceiling moved past
  100M once both landed.
- Led architecture and product decisions for large-scale data-visualization
  systems; established code-review and release processes that moved the
  team off continuous hotfixing toward predictable biweekly releases.
- **Internal enterprise AI platform** (details NDA): rebuilt the frontend as
  a **Next.js application orchestrating three retrieval backends** — an
  **MCP (Model Context Protocol)** service exposing raw operational data,
  plus two **RAG** services owned by other engineers on the team. The layer
  I didn't have access to turned out to be orchestration rather than data,
  and everything underneath it was reachable, so I re-implemented that
  routing and composition rather than waiting on repository access —
  working in a day. It replaced a **Chainlit**
  prototype, and I designed the surface for structured responses,
  citations, and inline data visualization rather than a chat wrapper.
- Tech: TypeScript, React, Next.js, MCP, Plotly, D3, Vite, Jest, Python.

## Meta (Facebook) — Senior Frontend Web Developer (contract via TEKsystems / Crystal Equation) — February 2019–December 2024

Joined to support the fast-growing **Small Business unit** — initially
managing its web presence solo, then helping the work scale into a
dedicated team of **eight web developers**, many of whom I personally
onboarded.

- Developed and maintained global-scale marketing platforms for Meta's
  Business audience — React and Hack interfaces on Meta's in-house CMS,
  balancing fast campaign delivery with accessibility, localization, and
  long-term maintainability across markets and languages.
- Launches include **Meta Creative Center** (2022–23), **Instagram
  Business Home** (2021), **Facebook Small Business Grants**, **Resource
  Hub**, and **"Boost with Facebook"** (2020).
- Introduced reusable CMS capabilities, wrote documentation and onboarding
  resources, interviewed frontend candidates across teams, and built an
  **email template infrastructure adopted by multiple teams** for global
  campaigns.

## Charlotte Russe — Lead Frontend Developer — February 2017–February 2019

Led frontend for CharlotteRusse.com, a fast-moving national eCommerce
business (Salesforce Commerce Cloud).

- **Managed and mentored a team of three frontend developers** (onshore
  and offshore), coordinating weekly production releases.
- Helped transition frontend development from external vendors in-house:
  new deployment and QA processes, technical documentation.
- Drove the 2018 **CharlotteRusse.com redesign**, modernizing the
  frontend from jQuery to ES6 while improving WCAG AA accessibility.

## Vitamin T (Aquent) — Web Developer, contract — January 2016–February 2017

Frontend contracting for clients including **Charlotte Russe** (which
converted into the lead role above), **IDEC**, and **CrunchBase**.

## AKQA — Creative Developer (2013–2015), Associate Creative Developer (2012–2013)

Interactive campaigns and product launches for global brands: **Apple
(iPhone 6 launch site)**, **Google**, **Nike**, **Audi**, **Levi's**,
**Target**, **Bud Light**, **Jordan**, **Salesforce**, **Visa (World Cup
2014)**.

- **Cannes Lions: Gold** (Design — Jordan NBA All Star, 2015), **Silver**
  (Social — Levi's #MAKEOURMARK, 2014), **Silver** (Mobile — Mobile
  Orchestra, 2013), plus a Bronze (Branded Tech — Levi's).
- Mobile Orchestra also earned Communication Arts Interactive Annual and
  FWA Mobile of the Day.
- Data-driven campaign UI: a d3.js live-score experience for Bud Light's
  March Madness campaign against a sports data API.

## Education

- **Academy of Art University** — BFA, Computer Arts and New Media
  (2008–2012), San Francisco.
- **General Assembly** — Product Management certification (2021).

## Earlier

Internships with Btrax and San Francisco International Airport;
independent digital work for entrepreneurs, local businesses, and
nonprofits. Fluent in the long arc from jQuery to React.
