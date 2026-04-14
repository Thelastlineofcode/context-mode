# context-mode — AGENTS.md

> ANN-Mesh parity repo. Canonical system spec: https://github.com/Thelastlineofcode/ANN-Mesh/blob/main/AGENTS.md

## Role in ANN-Mesh
Context lifecycle management across runtimes (Claude, Pi, openclaw).
Skill file: `.ann-core/skills/context-window-management.md`
Primary agents: **Ann** (orchestration) · **Scooter** (implementation) · **Noonie** (Levite context)

## Key Rules
- Load `context-window-management.md` skill before operating
- Boot: `ann health` → `ann context hydrate --agent [id]`
- Close loop: `ann context store` after every session
- No self-merges. Scooter opens PRs. Roids gates.
- Conventional commits only

## Connections
- rickd: `http://localhost:8080`
- ANN-Mesh: https://github.com/Thelastlineofcode/ANN-Mesh
