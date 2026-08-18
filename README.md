# Markdown from Git — How it works

Render Markdown files straight from your Git repository, natively inside any Jira issue — always in sync, no copy-paste.

## Overview
Markdown from Git displays Markdown files stored in a GitHub repository directly inside a Jira issue panel.
Content is rendered live from the source of truth, so there is no copy-paste and no manual sync.

## How it works
1. Open a Jira issue and add the **Markdown from Git** panel.
2. Enter the GitHub owner, repository, file path, and branch.
3. For private repositories, save a GitHub personal access token in the panel settings (stored encrypted in Forge storage).
4. The panel fetches the file from GitHub and renders it. Changes committed in Git appear on the next refresh.

## Key features
- Render any Markdown file (README, spec, runbook, ADR) from GitHub natively in Jira, with rich formatting — headings, tables, code blocks, and links.
- Pin to an exact file by owner, repository, path, and branch (ref).
- Supports private repositories via a per-user GitHub personal access token.

## Security & data handling
- Built on Atlassian Forge and runs on Atlassian-hosted infrastructure.
- Makes a single external call, to api.github.com, to fetch file contents.
- The GitHub personal access token is stored encrypted at rest in Forge storage and is used only to read the files you configure.

## Support
For questions or issues, contact DEVLOG Inc. (support details on the Marketplace listing).
