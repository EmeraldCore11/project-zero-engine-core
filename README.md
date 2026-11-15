# Project Zero

Project Zero is an extensible text-adventure platform for hosting creator-built worlds and adventures. It is designed around a protected, minimal engine core and a customizable experience layer.

## Repository role

This repository is the **master project repository**. It coordinates product requirements, governance, architecture, specifications, release planning, and integration across the Project Zero repositories.

## Architecture domains

1. **Platform Infrastructure** — identity, authorization, persistence, synchronization, search, notifications, moderation, audit, lifecycle, and other universal services.
2. **Protected Engine Core** — the minimal trusted boundary responsible for security, validation, isolation, authorization enforcement, persistence integrity, and controlled execution.
3. **Customizable Experience Layer** — worlds, adventures, characters, gameplay systems, user interfaces, themes, and creator/player modules.

## Authoritative documentation

The approved TDD, Master TDD, Master Specification Index, specification library, MSI, decision register, and release/implementation approvals are the sources of truth. Add the actual approved source documents here as they are consolidated. Do not replace missing source documents with summaries or invented requirements.

## Governance rules

- The original TDD requirements remain in force unless explicitly changed.
- Later decisions refine or extend earlier requirements; they must not silently erase them.
- Record conflicts and resolutions in the decision register.
- Product approval is not implementation authorization.
- A repository scaffold or Replit Agent instruction is not permission to implement features.
- Preserve traceability from requirements to specifications, decisions, and implementation stages.

## Repositories

- `project_zero` — master documentation, governance, planning, and integration.
- `project-zero-engine-core` — protected engine core (planned; repository not yet visible to the connected account).
- `project-zero-platform` — platform infrastructure and universal services.
- `project-zero-experience` — customizable worlds, adventures, gameplay, and UI.
- `project-zero-module-template` — reusable starter structure and guidance for modules.

## Current status

This is an initial repository scaffold. It does not represent a completed implementation plan, and it does not authorize implementation. Stage 0 readiness and implementation authorization must be handled explicitly.
