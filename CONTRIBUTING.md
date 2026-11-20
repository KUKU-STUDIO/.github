# Cómo contribuir a KUKU Studio

Este es el camino corto. Cada repo tiene su propio `CONTRIBUTING.md` y su onboarding con los comandos exactos: **ese manda** sobre este.

| Repo | Cómo contribuir | Onboarding |
|---|---|---|
| `kuku-board` | `CONTRIBUTING.md` | `docs/ONBOARDING.md` |
| `kuku-proyectos` | `CONTRIBUTING.md` | `docs/onboarding.md` |
| `kuku-app-template` | `CONTRIBUTING.md` | `docs/onboarding.md` |

Si eres una persona nueva, empieza por la [guía «Listo para operar»](https://github.com/KUKU-STUDIO/kuku-board/blob/main/docs/ready-to-operate.md).

(Los repos son privados: los enlaces solo abren para miembros de la organización.)

## Flujo con fork

1. Fork privado del repo en tu cuenta; clona tu fork y agrega el repo de la organización como `upstream`.
2. Rama `feature/<tema>` o `fix/<tema>` desde `upstream/main` (con tarjeta del Board: `feature/KB-<n>-<tema>`).
3. Corre la puerta local que describe el `CONTRIBUTING.md` del repo; guarda el exit code y los conteos de cada paso.
4. Abre el PR de tu fork a `main` con esa evidencia pegada.
5. Un mantenedor revisa y fusiona a mano los PR de forks (la CI no corre en forks).

## Reglas que no cambian

- Nadie hace push a `main`; todo entra por pull request.
- Commits en inglés con [Conventional Commits](https://www.conventionalcommits.org/); cada commit lleva sus tests y su documentación.
- Nada de `.env`, llaves, tokens, URLs con credenciales ni correos reales. Los ejemplos usan valores ficticios (`kb_EXAMPLE`, `123456`, `persona@example.com`).
- Labels: `type/*` (qué es), `area/*` (dónde), `priority/*`, y `good first issue`, `help wanted`, `onboarding`.
