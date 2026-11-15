# Project Zero Repository Map

This is the initial repository split. It establishes responsibility boundaries; it does not prescribe a premature microservice deployment or require every repository to become a separately deployed application.

| Repository | Responsibility | Boundary |
|---|---|---|
| `project_zero` | Product governance, requirements, specifications, decisions, roadmap, integration | Coordinates the whole product; does not absorb every implementation |
| `project-zero-engine-core` | Trusted engine boundary | Minimal protected responsibilities only |
| `project-zero-platform` | Universal platform capabilities | Shared services consumed through explicit contracts |
| `project-zero-experience` | Creator/player-facing experience systems | Replaceable and extensible modules outside the protected core |
| `project-zero-module-template` | Reusable module starter and authoring conventions | Template only; modules must declare contracts, dependencies, permissions, and compatibility |

## Dependency direction

- Experience modules must use documented platform/core interfaces rather than bypassing them.
- Platform services must not assume a particular world, genre, character system, or gameplay ruleset.
- The protected core must remain minimal and must not absorb optional gameplay systems.
- The module template must teach the approved interfaces; it must not create a second source of architectural truth.

## Important

This logical separation does not automatically mean separate runtime processes, services, deployments, or databases. Those decisions require explicit architecture and stage approval.
