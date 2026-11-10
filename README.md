# DSH Autonomous Worker

A general-purpose autonomous task execution Skill for **DeepSeek Harness (DSH)**.

It helps DSH turn an objective into a plan, discover available capabilities, compose tools, execute work, recover from failures, verify outputs, and report what was actually completed.

## What it is
- A reusable Skill/instruction package for DSH.
- Designed for research, analysis, operations, business workflows, documents, and software tasks.
- Adapts to capabilities actually available on the current machine.
- Supports macOS and Windows installation guidance.

## What it is not
- Not a standalone agent runtime, model, MCP server, or plugin.
- Does not create missing tools, credentials, permissions, or model access.
- Does not guarantee unattended execution where DSH or a tool requires approval.
- Does not bypass operating-system, application, or service permissions.

## Install
See [macOS installation](docs/INSTALL_MACOS.md) or [Windows installation](docs/INSTALL_WINDOWS.md). Copy `skills/dsh-autonomous-worker/` into a Skill directory recognized by your DSH installation, then refresh/restart DSH. Skill paths vary by DSH version/profile; do not assume a fixed path. See [Usage](docs/USAGE.md).

## Core operating rules
1. Inspect the current environment before planning.
2. Distinguish discovered, callable, invoked, and verified capabilities.
3. Prefer no-cost tools and models. Never silently switch to paid services.
4. Stop when a required quota is exhausted or a paid action would be needed.
5. Require human confirmation for consequential external actions.
6. Verify deliverables and label uncertainty, simulations, and failures.

## License
MIT. See [LICENSE](LICENSE).
