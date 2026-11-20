# KUKU Studio

KUKU es un estudio con una plataforma interna, **KUKU Board** (un ERP sobre Supabase), y apps independientes que se conectan a ella. Los repos son privados: los ven solo los miembros de la organización.

## Repos

| Repo | Para qué sirve | Stack |
|---|---|---|
| `kuku-board` | Núcleo del ERP: personas, roles, auditoría, gateway y SPA | Supabase (Postgres, Auth, Edge Functions) y Angular |
| `kuku-proyectos` | App de proyectos: tablero Scrum (esquema `proj`, tareas `KB-<n>`) y su API `proj-api` | Supabase y Deno |
| `kuku-app-template` | Plantilla para crear apps nuevas con el núcleo fijado por versión y una app demo `ping` | Supabase y Deno |

## Cómo empezar

1. **Invitación.** Aceptas la invitación a la organización y entras al equipo `developers` (rol Triage: lees, haces fork y comentas, no empujas al repo de la organización).
2. **Acceso al Board.** Recibes la invitación al KUKU Board por correo, haces el primer login y activas el TOTP.
3. **Fork.** Haces un fork privado del repo donde vas a trabajar.
4. **Clonar.** Clonas tu fork, agregas `upstream` y corres el setup local del repo.
5. **Primer PR.** Eliges un issue `good first issue`, abres el PR de tu fork a `main` y un mantenedor lo revisa y lo fusiona a mano.
6. **KB-n.** Tomas tu primera tarea real del Board (`KB-<n>`) y la enlazas con tu rama y tu PR.

Guía paso a paso, con comando y resultado esperado de cada paso: [`docs/ready-to-operate.md`](https://github.com/KUKU-STUDIO/kuku-board/blob/main/docs/ready-to-operate.md).

## Normas

- [Cómo contribuir](https://github.com/KUKU-STUDIO/.github/blob/main/CONTRIBUTING.md)
- [Política de seguridad](https://github.com/KUKU-STUDIO/.github/blob/main/SECURITY.md)
- Sin secretos, tokens ni datos de personas en issues, PR ni commits.
