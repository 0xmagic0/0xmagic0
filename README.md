## Security Advisories

| ID | Severity | Project | Issue |
|---|---|---|---|
| [CVE-2026-54052](https://github.com/czlonkowski/n8n-mcp/security/advisories/GHSA-j6r7-6fhx-77wx) | Critical (9.9) | czlonkowski/n8n-mcp | Cross-tenant access to workflow version backups in multi-tenant HTTP deployments |
| [CVE-2026-71963](https://www.vulncheck.com/advisories/hermes-agent-rce-via-git-core-fsmonitor-config-injection) | High | NousResearch/hermes-agent | Remote code execution via git `core.fsmonitor` config injection from an untrusted repository |
| [CVE-2026-46519](https://github.com/Flux159/mcp-server-kubernetes/security/advisories/GHSA-cr22-wjx7-2w6m) | High | Flux159/mcp-server-kubernetes | Tool access control bypass: presentation-layer filtering without execution-layer enforcement |
| [CVE-2026-72718](https://github.com/aaif-goose/goose/security/advisories/GHSA-r5pp-p5r8-466r) | High | aaif-goose/goose | Arbitrary command execution via `goose review` abusing git `core.fsmonitor` |
| [CVE-2026-77243](https://github.com/sooperset/mcp-atlassian/security/advisories/GHSA-3r68-hf9h-887v) | High | sooperset/mcp-atlassian | ENABLED_TOOLS / toolset authorization bypass |
| [CVE-2026-73496](https://github.com/sooperset/mcp-atlassian/security/advisories/GHSA-wm45-qh3g-v83f) | High | sooperset/mcp-atlassian | Arbitrary server-side file read via attachment upload |

## Research & Writeups

- [GitSpawn: A Single Flaw Lets Untrusted Repos Run Code in Claude Code, Codex, Cursor, and Grok](https://www.manifold.security/blog/ai-coding-agents-git-hijack)
- [Cursor CLI Ran Untrusted Repository Code With the Sandbox Switched Off](https://www.manifold.security/blog/cursor-cli-worktree-pre-trust-execution)
- [Anyone with an Account Could Run Commands on PewDiePie's AI Workspace (CVSS 9.9)](https://www.manifold.security/blog/odysseus-ai-workspace-rce)
- [The "Restricted" Deployment That Wasn't: Two Access-Control Bugs in community-built mcp-atlassian](https://www.manifold.security/blog/mcp-atlassian-access-control-bypass)
- [When Your AI Reviewer Works for the Attacker: A Confused-Deputy Bug in Microsoft's Azure DevOps MCP Server](https://www.manifold.security/blog/azure-devops-mcp-server-vulnerability)
- [CVE-2026-54052: A Wrong Number in n8n-mcp Leaked Your Neighbor's Credentials](https://www.manifold.security/blog/n8n-mcp-idor-cross-tenant-credential-theft)
- [When "Read-Only Mode" Isn't: CVE-2026-46519 in mcp-server-kubernetes](https://www.manifold.security/blog/mcp-server-kubernetes-readonly-bypass)
- [When HttpOnly Isn't Enough: Chaining XSS and GhostScript for Full RCE Compromise](https://www.praetorian.com/blog/httponly-cookie-bypass-xss-ghostscript-rce/)

## Tooling

- [agent2shell](https://github.com/0xmagic0/agent2shell) - Programmable reverse shell interface for AI agents. Catches reverse shells over TCP, exposes them via Unix sockets. Built in Go.
