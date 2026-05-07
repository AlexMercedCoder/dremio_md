# Dremio AI Agent Reference

This directory contains `DREMIO.md`, a highly-optimized, token-efficient reference file designed specifically to help AI agents and coding assistants understand the Dremio tool ecosystem.

## How to use `DREMIO.md`

`DREMIO.md` is formatted to give AI agents the exact context they need (the "what", "when", and "why") without wasting token context limits on lengthy explanations. It points the agent to the official documentation and repositories so they can dynamically learn how to use the best tool for the job.

### Best Practices for Prompting

When asking an AI agent (like ChatGPT, Claude, GitHub Copilot, or Antigravity) to interact with Dremio, include the contents of `DREMIO.md` in your system prompt or initial message. 

Here are examples of how to effectively prompt an agent using this file:

#### Example 1: Providing Context Directly (Chat Interfaces)
> "I need you to write a Python script that runs an ad-hoc SQL query against Dremio. Before you start, please review the following reference guide to determine the best tool to use, read its documentation, and then ask me for the necessary credentials safely:
> 
> [Paste contents of DREMIO.md here]"

#### Example 2: Referencing the File (Agents with Workspace Access)
> "Please write a Python script to interact with my Dremio Cloud instance. I want to use dataframe-like syntax. First, read `DREMIO.md` in this directory to identify the correct library to use. Read that library's documentation to understand how it handles authentication, tell me how to provide those credentials, and then write the script."

### Why this approach works
By injecting `DREMIO.md` into your workflow, you prevent the agent from:
- Hallucinating outdated or non-existent Dremio libraries.
- Using the wrong tool for the job (e.g., using the Software CLI for a Cloud instance).
- Wasting your token context window on full documentation pages, since the agent can independently follow the links to read exactly what it needs.
