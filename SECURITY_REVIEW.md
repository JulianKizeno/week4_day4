# Revisión de seguridad — 2026-10-24

Repositorio: `JulianKizeno/week4_day4`. Rama: `security/review-2026-10-24`.

## Correcciones

- Update vulnerable dependencies: mongoose ^6.13.12, Replace LibSass/node-sass with Dart Sass

## Auditoría npm después de los cambios

| Proyecto | Críticas | Altas | Moderadas | Bajas | Total |
|---|---:|---:|---:|---:|---:|
| `crud-app-read` | 0 | 0 | 0 | 0 | 0 |
| `get-request-info` | 0 | 0 | 0 | 0 | 0 |
| `post-request-info` | 0 | 0 | 0 | 0 | 0 |

## Verificación

- Inicialización de servidor (`get-request-info`) con APIs reales de las dependencias y conexión de base de datos aislada: correcta.
- Inicialización de servidor (`post-request-info`) con APIs reales de las dependencias y conexión de base de datos aislada: correcta.
- Inicialización de servidor (`crud-app-read`) con APIs reales de las dependencias y conexión de base de datos aislada: correcta.

## Límites y configuración

- La auditoría cubre el árbol npm resuelto, no demuestra ausencia de vulnerabilidades de lógica, infraestructura o servicios externos. No se ha desplegado ni fusionado este cambio.
- SCSS se compila al iniciar el servidor; reiniciar tras modificar estilos. Eliminar LibSass evita su árbol obsoleto de dependencias nativas.
