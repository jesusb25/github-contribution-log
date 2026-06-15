# Contribution [#]: Validate API inputs

**Contribution Number:** 1
**Student:** Jesus Ballesteros
**Issue:** [\[GitHub issue link\] ](https://github.com/issues/assigned?issue=zimicjs%7Czimic%7C477)
**Status:** Phase I Complete

---

## Why I Chose This Issue

This issue validates user inputs to ensure they follow expected formats and types. Since this is a public api this will help me dive into security and validation which is critical to large scale applications. I also want to learn how to write tests for validation logic and handle edge cases effectively.

## Understanding the Issue

### Problem Description

Zimic does not fully validate the inputs of the public API, such as checking if the parameters are of the expected types. We currently rely mostly on TypeScript to report such problems to users. However, this allows invalid values to be passed at runtime, possibly causing unexpected behavior. Zimic should validate each input to make sure it is correct, either being of the correct type or part of an expected enum.

### Expected Behavior

Users should receive clear error messages when they provide invalid inputs to the API, and the system should prevent any operations from proceeding with those invalid inputs.

### Current Behavior

Currently, if a user provides an invalid input, the system may throw a runtime error or behave unpredictably, which can lead to a poor user experience and potential security vulnerabilities.

### Affected Components

public API input validation logic, error handling mechanisms, and potentially any components that rely on user inputs.

---

## Reproduction Process

### Environment Setup

Issue is a feature request, so no specific environment setup is needed to reproduce.

### Steps to Reproduce

1. Attempt to call the public API with invalid inputs (e.g., wrong data types, missing required fields).
2. Observe the system's response (e.g., error messages, crashes, or unexpected behavior).
   Api documentation can be found [here](https://zimic.dev/docs/api).

### Reproduction Evidence

- **Commit showing reproduction:** [Link to commit in your fork]
- **Screenshots/logs:** [If applicable]
- **My findings:** [What you discovered during reproduction]

---

## Solution Approach

### Analysis

[Your analysis of the root cause - what's causing the issue?]

### Proposed Solution

[High-level description of your fix approach]

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** [Restate the problem]

**Match:** [What similar patterns/solutions exist in the codebase?]

**Plan:** [Step-by-step implementation plan]

1. [Modify file X to do Y]
2. [Add function Z]
3. [Update tests]

**Implement:** [Link to your branch/commits as you work]

**Review:** [Self-review checklist - does it follow the project's contribution guidelines?]

**Evaluate:** [How will you verify it works?]

---

## Testing Strategy

### Unit Tests

- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests

- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing

[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress

[What you built this week, challenges faced, decisions made]

### Week [Y] Progress

[Continue documenting as you work]

### Code Changes

- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**

- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
