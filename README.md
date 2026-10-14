# VGC Meta Analysis · Regulación M-C (Pokémon Champions)

Dashboard interactivo con el meta de la Regulación M-C, construido a partir del Top 32 de 10 torneos (320 equipos), del 13 de septiembre al 11 de octubre de 2026.

**Torneos:** regionales de Louisville, Baltimore, Frankfurt, Recife y Brisbane; VR Challenges de septiembre (#1, #2) y octubre (#1, #2); y ESM Madrid 2026 Clasificatorio 1.

## Pestañas

- **Uso:** uso por Pokémon en el Top 32 y en el Top 8.
- **Tendencias:** cómo sube o baja el uso fin de semana a fin de semana.
- **Conversión:** win rate en el campo completo de los VR Challenges frente a su presencia en Top 32 y Top 8.
- **Compañeros:** con qué Pokémon se suele llevar cada uno.
- **Sets:** movimientos, objeto, habilidad y naturaleza de cada Pokémon, y los sets completos más repetidos, comparando el total con el Top 8.
- **Objetos:** objetos de los 320 equipos.
- **Megas:** si cada mega va sola o con otra, cuántas veces llega al Top 8 y qué torneos ganó.
- **Arquetipos:** equipos agrupados por núcleo (comparten en promedio 4 de 6 Pokémon) y un índice de posicionamiento que pondera puesto, tamaño del torneo y recencia. Incluye los equipos individuales con mejor índice.
- **Por torneo:** megas por torneo.
- **Equipos y pastes:** los 320 equipos con su enlace a VR Pastes.

## Cómo verlo

Abre `index.html` en cualquier navegador; no hace falta cuenta ni instalar nada. Si GitHub Pages está activado, también se puede ver en `https://hector310595.github.io/VGCMetaAnalysis/`.

## Fuentes

victoryroad.pro, circuit.victoryroad.pro, esm.victoryroad.pro, VR Pastes y pokedata.ovh. Datos actualizados al 13 de octubre de 2026.

Los datos crudos están en `data/`:

- `equipos_mc.csv`: equipos.
- `arquetipos_mc.csv`: arquetipo, núcleo y flex de cada equipo.
- `sets_mc.csv`: un registro por Pokémon con objeto, habilidad, naturaleza y movimientos, leído de VR Pastes. Los pastes de torneo son Open Team List y no incluyen stat points.
- `winrates_vr.csv`: win rates.
