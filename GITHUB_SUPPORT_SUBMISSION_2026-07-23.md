# Resumen para GitHub Support

Use this as the body of your ticket at https://support.github.com/contact

---

**Subject:** Urgent - Unauthorized local file scanning, code copying, IP appropriation and privacy violation

**Account:** valeriasaa-lgtm

**Summary:**

I am Valeria Saa, the author of the Serena MCP project. Between June and July 2026 I detected that the Copilot/Codex agent (via the MCP protocol) scanned, copied and stored local files from my machine in its workspace, including:

- A private source file (`server.json`) from a local Serena/OraiOS snapshot.
- A non-technical decoy file containing personal conversations.
- Fragments of my artistic work in Norwegian.

I also observed automated git activity on my terminal (commit/push) targeting the `oraios/serena` repository without my authorization. In addition, my Penpot fork disappeared while an OraiOS fork remains active.

**Key evidence:**

- SHA-256 of the copied file: `cab9044bb9792014fe0645120e218d90c28ef4984492176b11ee635238d7c7e2`
- Original path: `/Users/valesa/Documents/SERENA/INVESTIGACION_DERIVACION_ORAIOS_SERENA_NO_PUBLICAR_20260603/repo_snapshots/oraios__serena/server.json`
- Copied path: `/Users/valesa/Documents/Codex/2026-06-20/files-mentioned-by-the-user-pasted/`
- Decoy file path: `/Users/valesa/Documents/Codex/2026-07-03/haceme-una-copia-de-todo-el/inputs/REVISION_PRIVADA_MATIAS_AUTO_PRELIMINAR_20260705.md`

**Actions requested:**

1. Preserve access logs (IP, user-agent, sessions) for `valeriasaa-lgtm`, `oraios/serena` and `oraios/penpot` from 2026-06-01 to present.
2. Audit OAuth apps and personal access tokens on my account.
3. Review and close suspicious active sessions.
4. Investigate automated commit/push activity from my account to `oraios/serena`.
5. Send a written response detailing measures taken.

I have a full incident report with hashes, screenshots and logs ready to share under confidentiality.

Thank you,  
Valeria Saa
