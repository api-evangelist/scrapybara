# Scrapybara (scrapybara)

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
