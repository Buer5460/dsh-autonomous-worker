# Usage

## When to invoke
Ask DSH to use `dsh-autonomous-worker` when the objective spans multiple steps or requires choosing among installed capabilities.

Example requests:
- Use dsh-autonomous-worker to research this topic, compare primary sources, and produce a cited briefing.
- Use dsh-autonomous-worker to inspect this dataset, validate it, and create an analysis report.
- Use dsh-autonomous-worker to plan and execute this workflow using the Skills and MCP tools already installed.

## Expected behavior
1. Inspect available capabilities.
2. State a concise plan and material assumptions.
3. Execute safe steps without asking for approval at every trivial action.
4. Pause for confirmation before consequential external actions.
5. Verify each deliverable and report exact paths/links.

## Harmless smoke test
Ask: Use dsh-autonomous-worker to create a short checklist for organizing a personal reading list. Do not access the network, install anything, call paid models, or modify external systems. Save nothing; just return the checklist and state which capabilities you actually used.

Expected: DSH classifies it as low risk, needs no external tools, returns a useful checklist, does not claim tools it did not invoke, and reports that no files or external state changed.

## Capability evidence
- Discovered: appears in a tool/Skill list.
- Callable: interface is available.
- Invoked: DSH actually called it.
- Verified successful: result was checked against the intended outcome.
