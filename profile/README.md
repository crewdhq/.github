<div align="center">

  <h1>✦ Crewd</h1>

  <p><strong>The package manager for prompt-defined AI agents, skills, and teams.</strong></p>

  <p>
    Compile reusable, versioned subagents and team coordination natively into <strong>Claude Code</strong>, <strong>Cursor</strong>, and <strong>Gemini CLI</strong>.
  </p>

  <p>
    <a href="https://crewd.dev"><img src="https://img.shields.io/badge/website-crewd.dev-black?style=flat-square" alt="Website"></a>
    <a href="https://crewd.dev/docs"><img src="https://img.shields.io/badge/docs-reference-blue?style=flat-square" alt="Docs"></a>
    <a href="https://github.com/crewdhq/crewd-cli"><img src="https://img.shields.io/badge/cli-v0.1.0-orange?style=flat-square" alt="CLI"></a>
    <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="License"></a>
  </p>

  <p>
    <a href="https://crewd.dev">Web Platform</a> •
    <a href="https://crewd.dev/docs">Documentation</a> •
    <a href="https://crewd.dev/explore">Explore Registry</a>
  </p>

</div>

---

### Quick Installation

Install the standalone `crewd` CLI:

```bash
# macOS / Linux (Homebrew)
brew install crewdhq/tap/crewd

# Standalone Shell Installer
curl -fsSL https://crewd.dev/install.sh | sh
```

---

### How It Works

1. **Initialize your repository**:
   ```bash
   crewd init
   ```
   Auto-detects active AI coding hosts in your codebase (`.claude/`, `.cursor/`, `GEMINI.md`) and configures `crewd.json`.

2. **Hire subagents or teams**:
   ```bash
   crewd hire @alice/reviewer
   # Or hire an entire squad:
   crewd hire team @acme/backend-squad
   ```
   Resolves transitive dependencies, downloads tamper-proof content-addressable blobs, and compiles prompt instructions into native host adapter formats.

3. **Teach local skills**:
   ```bash
   crewd teach @alice/reviewer @tools/pr-description
   ```
   Customizes an agent's capability specifically for your repository without modifying upstream manifests.

4. **Durable repo memory**:
   Learnings and architectural decisions are preserved in `.crewd/memory/<agent>.md` across version upgrades and promotions.

---

### Core Repositories

| Repository | Description |
| :--- | :--- |
| **[crewd.dev](https://github.com/crewdhq/crewd.dev)** | The web platform, package registry API, interactive versioning UI, and documentation hub. |
| **[crewd-cli](https://github.com/crewdhq/crewd-cli)** | The official Go CLI (`crewd`) for installing, compiling, promoting, and managing prompt-defined agents. |

---

<div align="center">
  <sub>Built with open standards for the multi-agent coding future. © 2026 Crewd</sub>
</div>
