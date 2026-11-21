# KUKÜ Studio

KUKÜ es un estudio con una plataforma interna, **KUKÜ Board** (un ERP sobre Supabase), y apps independientes que se conectan a ella. Los repos son privados: los ven solo los miembros de la organización.

## Objetivo

> "volver KUKU AI native aplicando todos los estandares y procesos de calidad y automatizados usando agentes de IA como herramienta e innovacion entre los demas servicios de KUKU"

## Cómo trabajamos

- **Agentes de IA como herramienta.** Escriben borradores de código, tests y docs; una persona responde por lo que se entrega.
- **Revisión humana.** Nada llega a `main` sin que una persona revise el PR.
- **CI como puerta.** Un PR se fusiona con la CI en verde; nadie hace push a `main`.
- **ISO/IEC 25010 como marco de calidad.** Cada regla de calidad cuelga de una característica de la norma y tiene un comando que la verifica.
- **Conventional Commits** en inglés y **PR pequeños**: un tema por PR.

## Repos

| Repo | Para qué sirve | Stack |
|---|---|---|
| `kuku-board` | Núcleo del ERP: personas, roles, auditoría, gateway y SPA | Supabase (Postgres, Auth, Edge Functions) y Angular |
| `kuku-proyectos` | App de proyectos: tablero Scrum (esquema `proj`, tareas `KB-<n>`) y su API `proj-api` | Supabase y Deno |
| `kuku-app-template` | Plantilla para crear apps nuevas con el núcleo fijado por versión y una app demo `ping` | Supabase y Deno |

## Primer día

1. **Invitación a la organización.** La aceptas y entras al equipo `developers` (rol Triage: lees, haces fork y comentas, no empujas al repo de la organización).
2. **Invitación al Board.** Llega por correo: creas tu contraseña y registras la app de autenticación (QR).
3. **Clonar.** Haces un fork privado del repo, lo clonas y agregas `upstream`.
4. **Levantar local.** `supabase start`, `npm ci` y `npm start` (con Docker encendido).
5. **Correr los tests** del repo antes de cambiar nada.
6. **Primer issue.** Eliges uno con la etiqueta `good first issue` y comentas que lo tomas.
7. **Primer PR.** Abres el PR de tu fork a `main`; un mantenedor lo revisa y lo fusiona a mano.

Guía paso a paso, con comando y resultado esperado de cada paso: [`docs/ONBOARDING.md`](https://github.com/KUKU-STUDIO/kuku-board/blob/main/docs/ONBOARDING.md) y [`docs/ready-to-operate.md`](https://github.com/KUKU-STUDIO/kuku-board/blob/main/docs/ready-to-operate.md).

## Enlaces

- [KUKÜ Board en producción](https://board.kukustudio.com.co) (acceso por invitación)
- [Runbooks](https://github.com/KUKU-STUDIO/kuku-board/tree/main/docs/runbooks)
- [Checklist de puesta en marcha](https://github.com/KUKU-STUDIO/kuku-board/blob/main/docs/ready-to-operate.md)
- [Cómo contribuir](https://github.com/KUKU-STUDIO/.github/blob/main/CONTRIBUTING.md)
- [Política de seguridad](https://github.com/KUKU-STUDIO/.github/blob/main/SECURITY.md)
- Sin secretos, tokens ni datos de personas en issues, PR ni commits.
