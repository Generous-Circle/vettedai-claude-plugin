# OpenAI plugin listing preparation

The portable package is in [`plugins/vettedai-openai`](plugins/vettedai-openai). It targets the existing VettedAI MCP endpoint and OAuth flow. The listing identifies the current operator as **Generous Circle Ltd, trading as VettedAI**, consistent with the current public Terms and Privacy Policy. Confirm the exact verified developer identity in the OpenAI Platform before submission.

## Included in the package

- Portable `plugin.json` and remote `mcp.json`
- Existing VettedAI square icon
- Required public product, support, privacy, and terms URLs
- Five positive and three negative MCP review prompts
- All-country targeting (`publication.countries: []`)
- Accurate subscription/credit disclosure and no-checkout declaration

The listing says an active VettedAI subscription is required and some actions use plan entitlements or credits already in the account; email enrichment consumes credits per lead. OpenAI's current plugin guidelines allow existing paid-account access and explanation of entitlement limits, while prohibiting subscription sales, digital-credit sales, checkout, or upgrade promotion inside plugins. This package does not link to checkout or a purchase page.

## Still required in the OpenAI Platform

1. Verify the publisher identity and its affiliation with Generous Circle Ltd.
2. Upload the package, connect the existing MCP server, and review the imported tool metadata and automated findings.
3. Verify the required website domain using the portal's current challenge.
4. Provide a dedicated reviewer account and project/candidate sample data through Review details. Do not put credentials in this repository or ZIP.
5. Run the five positive cases against that test account and confirm actual imported MCP tool names. The expected names in `plugin.json` are based on the VettedAI tool names currently exposed to this session; confirm exact names in the portal scan before submission.
6. Record and host an accessible walkthrough showing the tested flows. No demo recording URL is included yet because a real reviewer-accessible recording does not exist.
7. Confirm the current Privacy Policy clearly covers the candidate and recruiter data categories processed through ChatGPT/Codex, purposes, recipients, retention, and user controls.
8. Resolve required automated findings. Submitting for review and publishing an approved listing are separate steps; neither is performed by this package change.

Employment data is personal data. The reviewer walkthrough and product usage must keep a human recruiter responsible for decisions, and the privacy disclosures and data handling must match VettedAI's actual practices.
