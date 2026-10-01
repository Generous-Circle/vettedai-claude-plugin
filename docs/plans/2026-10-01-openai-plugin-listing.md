# VettedAI OpenAI Plugin Listing Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Prepare an OpenAI Agent Plugin package that connects ChatGPT and Codex to the existing VettedAI MCP endpoint for public directory review.

**Architecture:** Keep the existing Claude Code package unchanged and add a separate portable OpenAI package in this repository. The package points directly to the hosted Streamable HTTP MCP endpoint and reuses its existing OAuth flow; it contains only listing metadata, review cases, and brand assets. Dashboard connection, domain verification, reviewer access, demo recording, review submission, and publication are separate steps.

**Tech Stack:** OpenAI Agent Plugins 1.0 manifest, Streamable HTTP MCP configuration, JSON, PNG assets, ZIP archive.

**Delivery:** Source repository `Generous-Circle/vettedai-claude-plugin`; base branch `main`; task branch `feat/openai-plugin-listing`; isolated checkout at `/Users/USER/code/repos/vettedai-audition-supabase-version/.claude/worktrees/vettedai-openai-plugin-listing`. Push each completed commit promptly, then open a PR to `main` promptly. Do not merge the source PR or submit/publish the listing without the applicable review and authorization.

---

### Task 1: Add the portable plugin package

**Files:**
- Create: `plugins/vettedai-openai/plugin.json`
- Create: `plugins/vettedai-openai/mcp.json`
- Create: `plugins/vettedai-openai/assets/vettedai-icon.png`

Use the existing `https://www.vettedai.app/mcp` endpoint and the VettedAI square icon. Use publisher copy “Generous Circle Ltd, trading as VettedAI,” as confirmed by the user and current legal pages; verify the publisher identity in the OpenAI Platform before submission. Include all-country targeting and disclose the active-subscription requirement and credit-consuming actions. Keep secrets, app bindings, and portal-generated IDs out of the source upload.

### Task 2: Add initial MCP review cases and listing metadata

Add five distinct positive test cases and three unsupported-request boundaries based on the actual MCP tools and their current schemas. Use the existing VettedAI product, support, privacy, and terms pages. Include only verified URLs and actual server tool names; replace the reviewer-data placeholders and run each positive case using a dedicated reviewer account before submission. Leave the demo URL absent until a real, reviewer-accessible recording exists.

### Task 3: Validate and package

Validate JSON syntax, required listing fields, text lengths, category, icons, review-case counts/fields, MCP endpoint, URL reachability, and ZIP inventory. Keep the archive outside the package directory. Do not upload it until the package is complete and the user requests portal upload.

### Task 4: Complete portal review preparation

In the OpenAI Platform portal, verify the publisher, connect and scan the endpoint, verify the exact publisher listing name and imported tool metadata, complete domain verification, add secure reviewer access for a dedicated VettedAI test account, and attach a real recorded walkthrough. Resolve all automated findings before submitting for review. Keep submission for review separate from publication of an approved version.
