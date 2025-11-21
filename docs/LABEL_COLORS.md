# Label Organization Guide

## Label Categories
| Label Name | Category | Description |
|------------|----------|-------------|
| bug | issue-type | Something isn't working; use for defects and regressions |
| enhancement | issue-type | Request or implementation of a new feature or improvement |
| documentation | issue-type | Improvements or additions to docs, guides, or examples |
| question | issue-type | Information or clarification requested |
| duplicate | status | Issue/PR that duplicates an existing item |
| has repro | status | A reproducible case is provided or confirmed |
| platform:macos | platform | macOS-specific behavior, bugs, or support |
| platform:linux | platform | Linux-specific behavior, bugs, or support |
| platform:windows | platform | Windows-specific behavior, bugs, or support |
| area:core | area | Core application/runtime functionality |
| area:tools | area | Tooling layer: Search/Grep, Write/Edit, Bash, etc. |
| area:api | area | API layer, client/server communication and integrations |
| area:ide | area | IDE integrations and editor-specific behavior |
| area:model | area | Model behavior, output quality, interpretation |
| area:tui | area | Terminal UI rendering, input, shortcuts, status line |
| area:mcp | area | Model Context Protocol servers, tools, and connections |
| area:packaging | area | Packaging, installation, update workflows |
| area:security | area | Security, permissions, policies, and safety controls |
| area:auth | area | Authentication, credentials, and key management |
| memory | performance | Memory usage concerns and resource management |
| perf:memory | performance | Performance issues specifically related to memory |
| external | source | External dependency or environment-related issue |

## Usage Guidelines
- issue-type
  - Use for classifying the nature of the work item (bug, enhancement, documentation, question).
  - Apply one primary issue-type label per item when possible.
- status
  - Use to communicate workflow state or evidence (e.g., duplicate, has repro).
  - Combine with issue-type to clarify current handling.
- platform
  - Apply when the item is specific to macOS, Linux, or Windows.
  - Multiple platform labels are allowed if the issue spans more than one OS.
- area
  - Use to indicate the subsystem or domain impacted (core, tools, api, ide, model, tui, mcp, packaging, security, auth).
  - Prefer at least one area label to aid routing and triage.
- performance
  - Apply to issues focused on performance or memory concerns.
  - Use perf:memory for memory-specific performance problems; use memory for broader memory tracking items.
- source
  - Use external when the root cause or dependency lies outside the repository (e.g., third-party tools, environment constraints).

General tips
- Prefer precise labeling: combine one issue-type, one area, and any applicable platform and status labels.
- Avoid over-labeling; choose the most relevant labels while ensuring discoverability.
- Keep descriptions accurate and update this guide as labels evolve.