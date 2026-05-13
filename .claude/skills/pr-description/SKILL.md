---
name: pr-description
description: Writes pull request descriptions. Use when creating a PR, when the user asks for a PR description, says "write up this PR", "describe my changes", "help me open a pull request", or wants to document what's on their branch before merging. Also trigger when the user asks Claude to summarize branch changes in a way that could be shared with reviewers.
---

When writing a PR description:

1. Run `git diff main...HEAD` to see all changes on this branch
2. Also run `git log main...HEAD --oneline` to get a sense of the commit history
3. Write a description following this format:

## What
One sentence explaining what this PR does.

## Why
Brief context on why this change is needed.

## Changes
- Bullet points of specific changes made
- Group related changes together
- Mention any files deleted or renamed
