# CLAUDE.md

@AGENTS.md
@.claude/CLAUDE.md

This project uses [AGENTS.md](https://agents.md/) as the standard for providing context to AI coding agents. The `@AGENTS.md` import above tells Claude Code to load `AGENTS.md` automatically; other tools that natively support `AGENTS.md` will pick it up directly. The `@.claude/CLAUDE.md` import loads the local hard-rules file (gitignored) that mirrors the PostToolUse hook policy.
<!-- cloude-code-toolbox:mcp-skills-awareness-begin -->

### MCP & Skills awareness (Claude Code ToolBox)

_Last synced: 2026-11-22T04:47:28.614Z._

- **Full report:** `.claude/cloude-code-toolbox-mcp-skills-awareness.md` in this workspace (auto-overwritten on each scan). Use it as ground truth for configured servers and skill folders.
- **MCP:** For **live tools** in Claude Code, enable the matching server via `/mcp`. Servers are configured in `~/.claude.json` (user) and `.mcp.json` (project).
- **When the user’s task matches a server** (e.g. Confluence work and a **Confluence** / **Atlassian** MCP is listed), **prefer that server id** and plan on tool use—not only file search.
- **Skills:** Folders below contain `SKILL.md`; attach or cite paths in chat when relevant.

#### Workspace MCP

- `c:\Users\NEW\Documents\GitHub\langflow\.mcp.json` _(workspace: langflow)_ — _file missing_

_No active workspace servers in mcp.json._

#### User MCP

- `C:\Users\NEW\.claude.json` — _no servers defined_

_No active user-scoped servers in mcp.json._

#### Project skills

- **backend-code-review** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\backend-code-review` — Review backend code for quality, security, maintainability, and best practices based on established checklist rules. Use when the user requests a review, analysis, or improvement of backend files (e.g., `.py`) under the 

- **component-refactoring** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\component-refactoring` — Refactor high-complexity React components in Langflow frontend. Use when manual complexity assessment shows complexity > 50 or lineCount > 300, when the user asks for code splitting, hook extraction, or complexity reduct

- **e2e-testing** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\e2e-testing` — Write and review Playwright E2E tests for Langflow. Trigger when the user asks to write, fix, or review E2E tests, spec files, Playwright tests, or integration tests that exercise the full UI. Also trigger when modifying

- **frontend-code-review** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\frontend-code-review` — Review frontend code (.tsx, .ts, .js files) for quality, performance, and correctness against Langflow's frontend conventions. Supports pending-change reviews and file-targeted reviews.

- **frontend-i18n** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\frontend-i18n` — Add, change, or review user-facing text in the Langflow frontend using the i18n system (i18next / react-i18next). Use whenever a change adds or edits UI strings — labels, buttons, tooltips, modals, toasts, error messages

- **frontend-query-mutation** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\frontend-query-mutation` — Guide for implementing Langflow frontend query and mutation patterns with Axios and TanStack React Query v5. Trigger when creating or updating API hooks in controllers/API/queries, consuming UseRequestProcessor in compon

- **frontend-testing** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\frontend-testing` — Write, review, and debug Jest and React Testing Library unit and integration tests for Langflow frontend components, hooks, utilities, and Zustand stores.

- **ibm-a11y-level1-audit** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\ibm-a11y-level1-audit` — Perform a scoped IBM Equal Access Level 1 compliance audit of a chosen Langflow frontend surface (routes, components, or a PR) and produce a findings report mapped to WCAG/IBM Level 1 criteria. Default behavior is audit 

- **ibm-a11y-pr-remediation** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\ibm-a11y-pr-remediation` — Scan every frontend surface touched by the current PR/branch for IBM Equal Access Level 1 accessibility issues and fix all in-scope violations by default. Discovers changed files, maps them to routes/components/states, r

- **ibm-a11y-route-scan** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\ibm-a11y-route-scan` — Batch-scan Langflow frontend routes for accessibility issues using the Python IBM Equal Access scanner (scripts/a11y/a11y_scan.py) and produce JSON/Markdown/HTML reports. Scans the default-loaded state of each route only

- **ibm-a11y-testing-guide** — `c:\Users\NEW\Documents\GitHub\langflow\.agents\skills\ibm-a11y-testing-guide` — Reference guide for writing and running Langflow frontend accessibility tests with axe (Jest) and IBM Equal Access (Playwright `page.runA11yScan`). Covers which engine/test layer to pick, the POUR checklist, axe-vs-IBM r

#### User skills

- **bytestream-solution-author** — `C:\Users\NEW\.agents\skills\bytestream-solution-author` — |

<!-- cloude-code-toolbox:mcp-skills-awareness-end -->
