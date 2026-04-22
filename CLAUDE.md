# Context for Claude Code

This repo is part of Brian Way's AI workspace.

## Shared Knowledge

All persistent context, architecture docs, and process definitions live in the shared knowledge base:
```
~/ai-workspace/GitHub/ai-knowledge-base/
```

Before starting work, read `ai-knowledge-base/CLAUDE.md` for full workspace context, tool stack status, and active work items.

## Sync Protocol

After any notable change in this repo, update the shared knowledge base:
1. If a new tool or capability was built → update `ai-knowledge-base/CLAUDE.md` (Tool Stack / Active Work)
2. If a setup step changed → update `ai-knowledge-base/BOOTSTRAP.md`
3. If architecture changed → update the relevant doc in `ai-knowledge-base/pipeline/`
4. Commit and push changes to ai-knowledge-base so all tools stay in sync.
