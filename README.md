<div align="center">

# Turnip A6xx Drivers

**Drivers Vulkan Turnip para Adreno 6xx (Android)**

[Descargas](../../releases) · [Compatibilidad](docs/COMPATIBILIDAD.md) · [Reportar prueba](../../issues/new/choose)

</div>

---

## Drivers

Aquí publico drivers **Turnip** compilados para la serie **Adreno 6xx**, la que casi todos los autores han dejado de lado para centrarse en 7xx y 8xx. Base fija de Mesa, parches de estabilidad para esta familia y pruebas reales en gama baja, empezando por el **Adreno 610 (Snapdragon 680)**.

Todos los drivers están en [**Releases**](../../releases).

| Versión | Mesa base | Android | GPU probada | Descarga |
|---|---|---|---|---|
| **v27.0.0-R3** | `fdae82f0e23f` | 11+ | Adreno 610 | [Descargar](../../releases) |

## GPUs

| Serie | Adreno |
|---|---|
| Gama media/baja | 610, 612, 618, 619, 619L |
| Gama alta | 630, 640, 650, 660, 680, 690 |

Solo Adreno 6xx. Estado por GPU en [`docs/COMPATIBILIDAD.md`](docs/COMPATIBILIDAD.md).

## Qué incluyen

- Recuperación de contexto KGSL (solo gen 6).
- UBWC en imágenes mutables.
- Contador de memoria por proceso.
- Build optimizada, compatible con Android 11+.

## Resultados

| GPU | SoC | Android | Juego | FPS |
|---|---|---|---|---|
| Adreno 610 | Snapdragon 680 | 13 | T6 Requiem (BO2), texturas custom, FOV 120 | 20–40 |

## Problemas conocidos

- Algunas texturas desaparecen en T6 Requiem (A610). En investigación.
- Sin benchmarks medidos; el rendimiento depende del juego y del kernel KGSL del dispositivo.

## Créditos

Este proyecto no es un driver nuevo: es **Mesa** (Turnip/Freedreno) con parches de otros autores, recortado a A6xx. Base: receta de **StevenMXZ**. Lista completa en [`CREDITS.md`](CREDITS.md).

## Licencia

Parches bajo **GPLv3** ([`LICENSE`](LICENSE)). Mesa mantiene sus propias licencias (principalmente MIT). Proyecto no oficial, sin relación con Qualcomm, Mesa ni Google.
