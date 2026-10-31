# Chaotic Command documentation

This repository contains the Mintlify documentation for Chaotic Command.

**Published site:** https://chaoticcommand.mintlify.site/index

**Application repository:** https://github.com/Chaotic-Minds-Collective/Chaotic-Command

## Documentation audiences

- **Users:** Getting started, templates, custom structures, saved structures, AI-assisted design, previews, and applying approved setup changes.
- **Server owners:** Bot installation, bring-your-own-bot setup, safe operation, and recovery after partial progress.
- **Administrators:** Role permissions, channel visibility, and operational safety.
- **Developers:** Runtime architecture, local development, integrations, security, and project status.

## Local preview

Use Node.js 20.17.0 or newer and the Mintlify CLI.

\`\`\`bash
npm install -g mint
mint dev
\`\`\`

Run the commands from the directory containing \`docs.json\`. The local preview is available at \`http://localhost:3000\`.

## Publishing

The Mintlify deployment is connected to this repository's \`main\` branch. Changes merged to \`main\` can publish to the documentation site. Review all content and navigation changes before merging.

## Documentation standards

- Describe only behavior verified in the application repository or clearly label planned work.
- Keep user, server-owner, administrator, and developer instructions distinct.
- Never include tokens, secrets, private server identifiers, or personal credentials.
- Link to the application pull request or source file when it helps a developer verify behavior.
- Keep feature status and changelog aligned with the current application \`main\` branch.
