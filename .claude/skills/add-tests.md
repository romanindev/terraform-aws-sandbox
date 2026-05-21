# Skill: Add Tests

Use this skill when adding or improving tests.

## Steps

1. Identify the behavior that needs protection.
2. Choose the right test level:
    - unit;
    - integration;
    - component;
    - E2E.
3. Reuse existing test utilities where possible.
4. Add focused tests.
5. Avoid brittle implementation-detail tests.
6. Run the relevant test command if available.

## Rules

- Test behavior, not internal implementation details.
- Prefer clear test names.
- Avoid excessive mocking when integration tests would be more valuable.
- Do not chase coverage numbers blindly.

## Output

Summarize:

- What behavior is now covered.
- Which test files changed.
- Which commands were run.
- Any remaining gaps.