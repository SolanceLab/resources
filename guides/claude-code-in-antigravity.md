# Using Claude Code in Google Antigravity IDE

A guide for running Claude Code as your primary coding agent inside Google's Antigravity IDE — alongside its native Gemini integration, not instead of it.

**Written by Claude Code, running in Antigravity.** Yes, this guide was authored by the tool it documents.

---

## Why

Google Antigravity ships with Gemini 3 built in — free-tier access, deep IDE integration, solid for quick completions. But for complex multi-file refactoring, architectural planning, and agentic coding tasks, Claude Code with Opus remains the stronger agent.

You don't have to choose. Run both in the same workspace:

- **Gemini 3** for native IDE features — inline suggestions, quick explanations, chat
- **Claude Code** for heavy lifting — multi-step tasks, autonomous coding, MCP-connected workflows

Two models. One IDE. No conflict.

## What You Need

- **Google Antigravity** installed ([developer.android.com/antigravity](https://developer.android.com/antigravity))
- **Claude Pro or Max subscription** from Anthropic — this is what funds Claude Code usage

That's it. No API keys. No third-party proxies. No configuration files to hand-edit.

## How to Install

1. Open Antigravity
2. Go to the **Extensions** panel (left sidebar, or `Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for **Claude Code**
4. Click **Install**
5. When prompted, authenticate with your **Anthropic account** (the same one tied to your Pro or Max subscription)
6. Done

Claude Code appears in your sidebar. Open it and start working.

## Billing

This is the part every other guide gets wrong or ignores entirely.

- Claude Code usage bills against your **existing Claude Pro or Max subscription**
- It is **completely separate** from Antigravity's Gemini quotas
- Using Claude Code does not consume your Gemini free tier
- Using Gemini does not consume your Claude subscription
- There is no shared pool. They are independent billing systems from independent companies.

If you have a Claude Max subscription, you get the same Opus usage limits in Antigravity that you'd get in VS Code, the Claude desktop app, or any other supported environment.

## MCP Servers Carry Over

If you've configured MCP (Model Context Protocol) servers — for memory, Discord, Notion, databases, APIs, anything — they work identically in Antigravity.

Your `~/.claude/` configuration directory is shared across environments. Any MCP server that works in Claude Code on VS Code will work in Claude Code on Antigravity. No reconfiguration needed.

This also means any MCP servers you connect to Antigravity's native Gemini agent are available in the same workspace. Two agents, same tool access.

## What This Guide Is NOT

Every existing tutorial about Claude and Antigravity documents the same thing: how to route Antigravity's free Gemini API quotas through a proxy so you can use them as a Claude-compatible endpoint. That's the freeloading method — using Google's credits to call Claude-like models without paying Anthropic.

**This guide is not that.**

This documents the straightforward, legitimate path: you pay for a Claude subscription, you install the official extension, and you use it. No proxies. No credential juggling. No terms-of-service gray areas.

The reason this guide exists is that it's oddly underdocumented. The proxy method dominates search results because it's a hack, and hacks generate engagement. The simple path doesn't get written up *because* it's simple. But "install extension, log in" still needs to be said clearly once, so people know it's an option.

## Tips

- **Use Gemini for quick questions, Claude for complex tasks.** They complement each other well. Gemini's inline suggestions are fast; Claude Code's agentic mode handles multi-file operations.
- **Don't run both agents on the same task simultaneously.** They don't coordinate. Pick one per task.
- **Your Claude conversation history in Antigravity is local to that workspace.** It doesn't sync to claude.ai conversations.

---

*Guide created by House of Solance — Happy Valentine's Day, 14 February 2026*
