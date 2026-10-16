# Wordsearch en Español

A single-player Spanish-language word search toy. Players pick a themed category, hunt for its hidden words in a letter grid, and learn each word's definition as they find it.

## Language

**Categoría** (Category):
A themed set of 8 words a player searches for, e.g. *animales* or *colores*. Played independently of other categories, and tracks its own Mejor Tiempo.
_Avoid_: Theme, list, topic

**Palabra** (Word):
A single hidden entry within a Categoría that the player searches for in the Cuadrícula. Each Palabra has exactly one Definición.
_Avoid_: Term, entry, item

**Definición** (Definition):
The short Spanish-language explanation of a Palabra, revealed only once that word is found. For a Par País-Capital, the Definición of each half names the other half (e.g. Argentina's Definición is "Buenos Aires").
_Avoid_: Clue, description — "hint" is a distinct concept (see Pista)

**Par País-Capital** (Country-Capital Pair):
A linked relationship between one word in the *países* Categoría and one word in the *capitales* Categoría — e.g. Argentina / Buenos Aires. There are exactly 8 pairs; they're why those two categories can't be curated independently of each other.
_Avoid_: Match, link

**Cuadrícula** (Grid):
The 12×12 arrangement of letters generated fresh each time a Categoría is played, with its 8 Palabras placed horizontally, vertically, or diagonally — any of the 4 forward-reading directions (right, down, down-right, down-left), never reversed.
_Avoid_: Board, puzzle — "puzzle" is ambiguous between the Categoría and one instance of it; Cuadrícula names the instance

**Partida** (Play Session):
One attempt at a Categoría: a freshly generated Cuadrícula, played from an empty found-set to either completion or abandonment. Elapsed time is measured per Partida; only a completed Partida can set a new Mejor Tiempo.
_Avoid_: Game, round, attempt

**Selección** (Selection):
The sequence of grid cells a player drags or taps across in one continuous motion. A Selección becomes a Palabra Encontrada only if its cells spell one of the Categoría's 8 words along a straight, forward-reading line.
_Avoid_: Drag, swipe

**Palabra Encontrada** (Found Word):
A Palabra whose matching Selección has been made during the current Partida. Finding it triggers its Definición popup immediately.
_Avoid_: Match, hit

**Mejor Tiempo** (Best Time):
The fastest completion time ever recorded for a Categoría, independent of which random Cuadrícula layout produced it. Stored per Categoría, not per Cuadrícula.
_Avoid_: Record, high score, personal best

**Pista** (Hint):
An automatic, un-requested reveal of one not-yet-found Palabra's full path in the Cuadrícula, shown for about a second. Fires after 5 minutes without a new Palabra Encontrada in the current Partida, and can re-fire every subsequent 5 minutes of continued inactivity.
_Avoid_: Clue
