# VGC Meta Analysis · Regulación M-C (Pokémon Champions)

Dashboard interactivo con el meta de la Regulación M-C, construido a partir del Top 32 de 16 torneos (493 equipos), del 13 de septiembre al 25 de octubre de 2026. Incluye sprites de Pokémon Champions (vía PokeAPI) en las secciones de uso, arquetipos, tendencias, megas y equipos.

**Torneos:** regionales de Baltimore, Frankfurt, Brisbane, Recife, Louisville, Nice y Puebla; VR Challenges de septiembre (#1, #2) y octubre (#1 a #4); ESM Madrid 2026 Clasificatorios 1 y 2; y el Top 16 del Thailand Premier Ball League.

## Pestañas

- **Uso:** uso por Pokémon en el Top 32 y en el Top 8.
- **Arquetipos:** familias de equipos con nombre (Y-Chu Balance, Delphox Balance, Sun Rain, Gengar Perish, Goli Rain…), cada una con su núcleo fijo, segunda mega, piezas frecuentes y variables (con su función y qué gana o pierde), índice de posicionamiento, evolución semanal y equipos destacados agrupados cuando son el mismo equipo.
- **Matchups:** quién le gana a quién entre arquetipos (6 VR Challenges y 2 clasificatorios ESM, ajustado por la fuerza de los jugadores).
- **Tendencias:** uso por fin de semana y qué sube o baja. Incluye "Acción y reacción" (cambios del meta con hipótesis, confianza y lo que no encaja) y la evolución semanal de movimientos y objetos por Pokémon.
- **Megas:** uso de cada mega, cuáles llegan al Top 8 y combinaciones de megas.
- **Rendimiento:** uso frente a win rate en el campo completo (gráfica con sprites) y qué Pokémon llegan más lejos de lo que su uso sugiere.
- **Sets:** movimientos, objeto, habilidad y naturaleza de cada Pokémon, lo que más rinde en su Top 8, sets completos y objetos más usados.
- **Compañeros:** con quién se lleva cada Pokémon.
- **Herramientas:** Tailwind, Trick Room, climas, Wide Guard, prioridad… de septiembre a octubre.
- **Stat points:** escalera de velocidades y spreads publicados (VGCPastes Repository).
- **Equipos:** ficha de cada torneo y los equipos con su paste.

## Tres equipos recomendados

`equipos.html` propone tres equipos basados en pastes campeones (Raichu-Y + Garchomp-Z, Sol y lluvia, Floette + Dragonite-Mega), con paste copiable, plan de juego y cambios justificados con datos. Cada equipo incluye:

- **Matchups:** récord contra rivales que llevan cada Pokémon en 3,973 partidas de los cuatro VR Challenges, y diferencia frente a lo esperado según la fuerza de ambos jugadores.
- **Cálculos clave:** daño con @smogon/calc (nivel 50, 1 stat point = 8 EVs) contra los sets más comunes publicados, y ajustes de stat points que aguantan golpes concretos sin perder velocidad.

## Cómo verlo

Abre `index.html` (dashboard) o `equipos.html` (equipos recomendados) en cualquier navegador; no hace falta cuenta ni instalar nada. Si GitHub Pages está activado, también se puede ver en `https://hector310595.github.io/VGCMetaAnalysis/` y `https://hector310595.github.io/VGCMetaAnalysis/equipos.html`.

## Fuentes

victoryroad.pro, circuit.victoryroad.pro, esm.victoryroad.pro, VR Pastes y pokedata.ovh. Datos actualizados al 25 de octubre de 2026; stat points hasta el 26 de octubre.

Los datos crudos están en `data/`:

- `equipos_mc.csv`: equipos.
- `arquetipos_mc.csv`: arquetipo, núcleo y flex de cada equipo.
- `spreads_mc.csv`: 1,314 sets con stat points y stats finales a nivel 50 (fuente: VGCPastes Repository, pokepast.es).
- `sets_mc.csv`: un registro por Pokémon con objeto, habilidad, naturaleza y movimientos, leído de VR Pastes. Los pastes de torneo son Open Team List y no incluyen stat points.
- `winrates_vr.csv`: win rates del campo completo por Pokémon (6 VR Challenges y 2 clasificatorios ESM).
- `partidas_vr.csv`: 3,973 partidas de los VR Challenges de septiembre y octubre, con el equipo de cada jugador (Pokémon y mega) y el marcador en juegos.
- `matchups_arquetipos.csv`: partidas, victorias reales y esperadas, y juegos ganados y perdidos entre cada par de arquetipos.
- `matchups_equipos.csv`: récord de los tres equipos recomendados contra rivales que llevan cada Pokémon o estilo (psyspam, lluvia, sol, arena, nieve, Prankster).
