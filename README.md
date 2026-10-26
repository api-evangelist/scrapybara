# Scrapybara (scrapybara)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Scrapybara provides virtual desktops for AI agents - remote Ubuntu, browser, and Windows instances that computer-use models can see and control. A single x-api-key REST API starts and manages cloud instances, streams the desktop, runs computer / keyboard / mouse actions, drives Chromium over Playwright CDP, executes bash and code, manages the filesystem and Jupyter notebooks, and saves reusable browser auth states.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/scrapybara/refs/heads/main/apis.yml)

## Tags

- AI Agents
- Virtual Desktops
- Computer Use
- Browser Automation
- Code Execution

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Scrapybara Instances API

Start, get, list, stop, pause, and resume cloud instances of type ubuntu, browser, or windows, with configurable timeout hours, blocked domains, and screen resolution. Paused instances preserve state and can be resumed later.

- **Human URL:** [https://docs.scrapybara.com/api-reference/start](https://docs.scrapybara.com/api-reference/start)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Instances
- Virtual Desktops
- Ubuntu
- Browser
- Windows

#### Properties

- [Documentation](https://docs.scrapybara.com/api-reference/start)
- [API Reference](https://docs.scrapybara.com/api-reference/start)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Computer Actions API

Drive a running desktop the way a human would - take a screenshot, get the interactive stream URL, and run computer actions (move mouse, click, drag, scroll, type text, press key combinations, wait) that computer-use models call directly.

- **Human URL:** [https://docs.scrapybara.com/ubuntu](https://docs.scrapybara.com/ubuntu)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Computer Use
- Screenshot
- Mouse
- Keyboard
- Streaming

#### Properties

- [Documentation](https://docs.scrapybara.com/ubuntu)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Browser API

Start and stop a Chromium browser on an instance, retrieve its Playwright Chrome DevTools Protocol (CDP) URL for programmatic control, read the current URL, and authenticate the browser with a previously saved auth state.

- **Human URL:** [https://docs.scrapybara.com/browser](https://docs.scrapybara.com/browser)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Browser Automation
- Playwright
- CDP
- Chromium

#### Properties

- [Documentation](https://docs.scrapybara.com/browser)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Code Execution API

Run bash commands and execute arbitrary code against a named kernel on an instance, capturing stdout, stderr, and results for agent workflows and data processing.

- **Human URL:** [https://docs.scrapybara.com/code-execution](https://docs.scrapybara.com/code-execution)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Code Execution
- Bash
- Sandbox

#### Properties

- [Documentation](https://docs.scrapybara.com/code-execution)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Filesystem API

Read, write, list, and manipulate files on an instance via file and edit actions, and upload binary files directly into the instance filesystem for agents to operate on.

- **Human URL:** [https://docs.scrapybara.com/filesystem](https://docs.scrapybara.com/filesystem)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Filesystem
- Files
- Upload
- Edit

#### Properties

- [Documentation](https://docs.scrapybara.com/filesystem)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Notebook API

Create and manage Jupyter notebooks on an instance - list kernels, create and delete notebooks, add cells, and execute individual cells or the whole notebook.

- **Human URL:** [https://docs.scrapybara.com/notebooks](https://docs.scrapybara.com/notebooks)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Jupyter
- Notebooks
- Kernels

#### Properties

- [Documentation](https://docs.scrapybara.com/notebooks)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Auth States API

Save the current browser session as a reusable auth state, list saved auth states, and modify them, so agents can skip repeated logins by replaying cookies and local storage across instances.

- **Human URL:** [https://docs.scrapybara.com/browser#auth-states](https://docs.scrapybara.com/browser#auth-states)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Auth States
- Sessions
- Cookies

#### Properties

- [Documentation](https://docs.scrapybara.com/browser#auth-states)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Scrapybara Environment API

Get, set, and delete environment variables on a running instance so agents and executed code can read API keys and configuration at runtime.

- **Human URL:** [https://docs.scrapybara.com/environment-variables](https://docs.scrapybara.com/environment-variables)
- **Base URL:** `https://api.scrapybara.com/v1`

#### Tags

- Environment Variables
- Configuration
- Secrets

#### Properties

- [Documentation](https://docs.scrapybara.com/environment-variables)
- [OpenAPI](openapi/scrapybara-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/scrapybara.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/scrapybara.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/scrapybara)
- [LinkedIn](https://www.linkedin.com/company/scrapybara)
- [Website](https://scrapybara.com/)
- [Documentation](https://docs.scrapybara.com)
- [Plans](plans/scrapybara-plans-pricing.yml)
- [Rate Limits](rate-limits/scrapybara-rate-limits.yml)
- [Fin Ops](finops/scrapybara-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
