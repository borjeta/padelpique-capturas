# padelpique-capturas

Automatiza las capturas de pantalla de la ficha de App Store de **PadelPique** (iPhone 6,9", 1320×2868, español e inglés):
instala el build de simulador en un runner macOS de GitHub Actions y lo recorre con [Maestro](https://maestro.dev).

- `capturas-ios/`: flows de Maestro (`01-capturas.yaml` y `sub/`).
- `.github/workflows/capturas.yml`: arranca el simulador, instala la app y ejecuta el flujo. Se lanza a mano (`workflow_dispatch`).
- Secretos del repositorio: `APP_URL` (`.tar.gz` del build `simulator` de EAS) y `DEMO_CODE` (código del grupo demo).

Este repositorio es público solo para usar minutos gratuitos de macOS; no contiene código de la app.
