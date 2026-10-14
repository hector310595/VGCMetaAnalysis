# VGC Meta Analysis · Regulación M-C (Pokémon Champions)

Dashboard interactivo con el meta de la Regulación M-C, construido a partir del Top 32 de 10 torneos (320 equipos), del 13 de septiembre al 11 de octubre de 2026.

**Torneos:** regionales de Louisville, Baltimore, Frankfurt, Recife y Brisbane; VR Challenges de septiembre (#1, #2) y octubre (#1, #2); y ESM Madrid 2026 Clasificatorio 1.

## Pestañas

- **Uso:** uso por Pokémon en el Top 32 y en el Top 8.
- **Tendencias:** cómo sube o baja el uso fin de semana a fin de semana.
- **Conversión:** win rate en el campo completo de los VR Challenges frente a su presencia en Top 32 y Top 8.
- **Compañeros:** con qué Pokémon se suele llevar cada uno.
- **Sets:** movimientos, objeto, habilidad y naturaleza de cada Pokémon, y los sets completos más repetidos, comparando el total con el Top 8.
- **Adaptaciones:** herramientas del meta (Tailwind, Trick Room, climas, Wide Guard, prioridad…) y su evolución de septiembre a octubre; techs que aparecen más en el Top 8 que en el resto, con una señal de fiabilidad estadística; y variantes de cada arquetipo con el set del mejor clasificado.
- **Stat points:** velocidades del meta (mín., moda y máx. por Pokémon) y spreads más repetidos, a partir de 199 equipos con resultado cuyos jugadores publicaron el paste completo (VGCPastes Repository).
- **Objetos:** objetos de los 320 equipos.
- **Megas:** si cada mega va sola o con otra, cuántas veces llega al Top 8 y qué torneos ganó.
- **Arquetipos:** equipos agrupados por núcleo (comparten en promedio 4 de 6 Pokémon) y un índice de posicionamiento que pondera puesto, tamaño del torneo y recencia. Incluye los equipos individuales con mejor índice.
- **Por torneo:** megas por torneo.
- **Equipos y pastes:** los 320 equipos con su enlace a VR Pastes.

## Tres equipos recomendados

`equipos.html` propone tres equipos basados en pastes campeones (Raichu-Y + Garchomp-Z, Sol y lluvia, Floette + Dragonite-Mega), con paste copiable, plan de juego y cambios justificados con datos. Cada equipo incluye:

- **Matchups:** récord contra rivales que llevan cada Pokémon en 3,973 partidas de los cuatro VR Challenges, y diferencia frente a lo esperado según la fuerza de ambos jugadores.
- **Cálculos clave:** daño con @smogon/calc (nivel 50, 1 stat point = 8 EVs) contra los sets más comunes publicados, y ajustes de stat points que aguantan golpes concretos sin perder velocidad.

## Cómo verlo

Abre `index.html` (dashboard) o `equipos.html` (equipos recomendados) en cualquier navegador; no hace falta cuenta ni instalar nada. Si GitHub Pages está activado, también se puede ver en `https://hector310595.github.io/VGCMetaAnalysis/` y `https://hector310595.github.io/VGCMetaAnalysis/equipos.html`.

## Fuentes

victoryroad.pro, circuit.victoryroad.pro, esm.victoryroad.pro, VR Pastes y pokedata.ovh. Datos actualizados al 14 de octubre de 2026.

Los datos crudos están en `data/`:

- `equipos_mc.csv`: equipos.
- `arquetipos_mc.csv`: arquetipo, núcleo y flex de cada equipo.
- `spreads_mc.csv`: 1,194 sets con stat points y stats finales a nivel 50 (fuente: VGCPastes Repository, pokepast.es).
- `sets_mc.csv`: un registro por Pokémon con objeto, habilidad, naturaleza y movimientos, leído de VR Pastes. Los pastes de torneo son Open Team List y no incluyen stat points.
- `winrates_vr.csv`: win rates.
- `partidas_vr.csv`: 3,973 partidas de los VR Challenges de septiembre y octubre, con el equipo de cada jugador (Pokémon y mega) y el marcador en juegos.
- `matchups_equipos.csv`: récord de los tres equipos recomendados contra rivales que llevan cada Pokémon o estilo (psyspam, lluvia, sol, arena, nieve, Prankster).
