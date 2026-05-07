# DevOps Portfolio —  Path

Demostración del flujo Gitflow aplicado a scripts de administración Linux.

## Flujo de trabajo

| Rama | Propósito | Se crea desde | Merge hacia |
|---|---|---|---|
| `main` | Código en producción | — | — |
| `develop` | Integración continua | `main` | `main` (via release) |
| `feature/*` | Nuevas funcionalidades | `develop` | `develop` (via PR) |
| `release/*` | Preparación de versión | `develop` | `main` + `develop` |
| `hotfix/*` | Correcciones urgentes | `main` | `main` + `develop` |

