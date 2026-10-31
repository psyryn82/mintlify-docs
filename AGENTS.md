# Chaotic Command documentation agent instructions

This repository contains the Mintlify documentation for Chaotic Command. Read these instructions before editing pages or navigation.

## Sources of truth

- Application code: https://github.com/Chaotic-Minds-Collective/Chaotic-Command
- Application implementation source of truth: the application's `main` branch.
- Documentation source of truth: this repository's `main` branch.
- Published documentation: https://chaoticcommand.mintlify.site/index

Verify application behavior against code and merged pull requests before documenting it. Do not treat a design mockup, old branch, proposal, or unmerged pull request as released functionality.

## Product terminology

- Use **Chaotic Command** for the product.
- Use **Discord server** or **server** for a Discord guild.
- Use **server owner** for the person responsible for the community.
- Use **administrator** for a person managing roles, permissions, and operations.
- Use **personal bot** or **customer-owned bot** for a bot connected by an end user.
- Use **shared bot** for the optional operator-configured bot.
- Use **preview** for the proposed setup plan before any Discord write.
- Use **audit** for the read-only inventory and supported findings.

## Documentation audiences

Maintain distinct guidance for:
- End users.
- Server owners.
- Administrators.
- Developers and operators.

Customer-facing pages should explain actions available through the current application. Developer pages may cover architecture, environment setup, storage, testing, integration boundaries, and operational constraints.

## Accuracy and safety rules

- Never describe planned or unmerged features as available.
- The current app adds structure inside an existing Discord server. It does not create a new Discord guild.
- The existing-server audit is read-only.
- Full move, rename, reorder, delete, and permission-edit operations are not implemented.
- The current AI workflow is a manual prompt and JSON handoff. The app does not call an AI provider.
- The active runtime uses direct Discord REST requests. A Composio adapter is not implemented.
- The app's operation lock is process-local. Do not claim multi-process safety.
- Automated tests use mocked Discord responses and offline fixtures. Do not describe them as live Discord acceptance.
- Never include tokens, client secrets, session secrets, database contents, private server IDs, or other credentials.
- Do not recommend Administrator permission as a workaround. The current bot permission request is Manage Channels and Manage Roles.

## Writing style

- Use active voice and second person for user instructions.
- Use sentence case for headings.
- Keep sentences concise and specific.
- Bold UI labels and use code formatting for paths, commands, and environment variable names.
- Avoid marketing claims that exceed verified functionality.
- Keep the feature-status page and changelog synchronized with the application's merged `main` branch.

## Change workflow

1. Read the existing page before editing it.
2. Verify behavior in the application repository.
3. Prefer targeted edits to existing pages.
4. Update navigation when adding a page.
5. Check internal links and page metadata.
6. Record the source commit or pull request for significant implementation updates.
7. Do not publish documentation or merge a pull request unless explicitly authorized.
