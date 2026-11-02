# VGC Meta Analysis · Regulación M-C (Pokémon Champions)

Dashboard interactivo con el meta de la Regulación M-C, construido a partir del Top 32 de 17 torneos (525 equipos), del 13 de septiembre al 1 de noviembre de 2026, y del campo completo (todas las partidas) de 6 VR Challenges, 2 clasificatorios ESM y los 8 regionales.

**Torneos:** regionales de Baltimore, Frankfurt, Brisbane, Recife, Louisville, Nice, Puebla y Gdańsk; VR Challenges de septiembre (#1, #2) y octubre (#1 a #4); ESM Madrid 2026 Clasificatorios 1 y 2; y el Top 16 del Thailand Premier Ball League.

## Secciones

- **Resumen:** familias que suben y bajan, mega del momento, último campeón y las noticias más recientes (ordenadas por fecha y solidez).
- **Meta:** uso, megas, herramientas (Tailwind, Trick Room, climas…) y rendimiento (uso frente a win rate en el campo completo).
- **Equipos:**
  - **Familias:** tarjetas con el núcleo resaltado (brillo dorado) y una ficha por familia: núcleo, contra quién gana y pierde, cuánto llega al Top 32, mejores equipos, noticias y cómo se arma (combinaciones de megas y piezas, con su efecto en el win rate).
  - **Matchups:** quién le gana a quién entre familias y resumen por familia (win rate, vs esperado y "llega al Top 32").
  - **Torneos:** ficha de cada torneo con Top 8, corte final, familias del campo completo frente al Top 32 y todos los equipos.
- **Pokémon:** ficha de cada Pokémon (sets, compañeros, por forma) y velocidad y stat points.
- **Tendencias:** noticias fechadas con dato, hipótesis y lo que falta comprobar (filtrables por solidez y texto), uso por fin de semana y evolución de sets.

Cualquier equipo se puede tocar para ver sus sets completos. Hay un buscador global (Pokémon, familia, jugador o torneo) y un glosario.

## Cómo verlo

Abre `index.html` en cualquier navegador; no hace falta cuenta ni instalar nada. Si GitHub Pages está activado, también se puede ver en `https://hector310595.github.io/VGCMetaAnalysis/`.

## Fuentes

victoryroad.pro, circuit.victoryroad.pro, esm.victoryroad.pro, VR Pastes y pokedata.ovh. Datos actualizados al 1 de noviembre de 2026; stat points hasta el 26 de octubre. El campo completo de los regionales (listas abiertas y emparejamientos) viene de pokedata.ovh.

Los datos crudos están en `data/`:

- `equipos_mc.csv`: equipos.
- `arquetipos_mc.csv`: familia, variante, núcleo y flex de cada equipo del Top 32.
- `spreads_mc.csv`: 1,314 sets con stat points y stats finales a nivel 50 (fuente: VGCPastes Repository, pokepast.es).
- `sets_mc.csv`: un registro por Pokémon con objeto, habilidad, naturaleza y movimientos, leído de VR Pastes. Los pastes de torneo son Open Team List y no incluyen stat points.
- `winrates_vr.csv`: uso y win rate del campo completo por Pokémon y torneo (6 VR Challenges, 2 clasificatorios ESM y 8 regionales).
- `partidas_vr.csv`: 3,973 partidas de los VR Challenges de septiembre y octubre, con el equipo de cada jugador (Pokémon y mega) y el marcador en juegos.
- `matchups_arquetipos.csv`: partidas, victorias reales y esperadas, y juegos ganados y perdidos entre cada par de arquetipos.
- `matchups_equipos.csv`: récord de los tres equipos recomendados contra rivales que llevan cada Pokémon o estilo (psyspam, lluvia, sol, arena, nieve, Prankster).
- `matchups_familias.csv`: partidas, victorias reales y esperadas entre cada par de familias (VR, ESM y regionales, sin espejos en el resumen).
- `anatomia_arquetipos.csv`: núcleo, combinaciones de megas y piezas de cada familia, con win rate frente al resto de la familia.
- `familias_por_torneo.csv`: por regional, inscritos, Top 32, Top 8 y partidas de cada familia en el campo completo.
- `corte_final.csv`: resultados del corte final de los 8 regionales (por puesto final).
