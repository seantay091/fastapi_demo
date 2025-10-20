# Automated Issue Comment — How to use @claude code actions

This comment is added to new Issues to help contributors quickly request actionable work from Claude using concise, consistent prompts.

## How to invoke
- Mention the assistant and a short action: `@claude <action>`.
- Be specific: include target file(s), desired behavior, and any constraints (style guide, tests, target branch).
- If you want a particular coding style or reference file, name it (for example: "same coding style as `main.py`").

## Useful prompt patterns
- Implementation: `@claude implement <feature> in <file> using the same coding style as main.py`
- Review: `@claude review the PR and highlight any missing documents or potential failing code`
- Tests: `@claude add unit tests for <function> in <file> covering edge cases <list>`
- Bugfix: `@claude reproduce the bug described above and propose a minimal fix in <file>`
- Refactor: `@claude refactor <module> to <goal> while preserving public API and add tests`
- Docs: `@claude generate README section with usage examples for <feature>`
- Security check: `@claude audit code in <path> for XSS/SQL injection and suggest fixes`

## Examples (copyable)
- `@claude implement a calendar widget using the same coding style as main.py`
- `@claude review the PR and highlight any missing documents or potential failing code`
- `@claude add unit tests for parse_date in src/utils.py covering invalid and timezone cases`

## Best practices for prompts
- Provide a minimal reproducible example or point to the exact files/lines.
- State the language/framework and any style guide to follow.
- Describe acceptance criteria (expected behavior, performance limits, or test pass criteria).
- Ask for small, focused changes per request to keep reviews concise.
- If you want a code change applied as a patch/PR, indicate target branch and commit message format.

## What Claude will return
- A clear plan of changes, diffs/patches or suggested code, test additions, and a short rationale.
- Notes on any assumptions and follow-up steps to validate the change.

Use these patterns to get fast, actionable contributions from Claude for implementation, review, tests, docs, and security audits.
