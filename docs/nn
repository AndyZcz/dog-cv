## HRNet – „High-Resolution Network“
HRNet je konvoluční neuronová síť, která udržuje vysoké prostorové rozlišení během celého průchodu sítí místo toho, 
aby obraz nejdříve silně zmenšovala a pak opět zvětšovala. To znamená, že si zachovává detaily.

Síť má paralelně běžící větve na různých rozlišeních, které si navzájem vyměňují informace (tzv. multi-scale feature fusion). 
To umožňuje kombinovat kontext (větší oblasti obrazu) i jemné detaily současně.

HRNet se často používá jako top-down metoda.

## PifPaf – Composite Fields
PifPaf je jiný typ modelu pro detekci klíčových bodů, který vznikl jako bottom-up metoda. 
To znamená, že nejprve odhadne všechny klíčové body na obrázku a pak je spojí do jednotlivých osob, bez potřeby detekovat obdélníky osob dopředu.

Má dva druhy polí:
Part Intensity Fields (PIF): předpovídají pravděpodobnost pozice kloubu a jeho přesnou koordinátu.
Part Association Fields (PAF): reprezentují, jak spolu různé klouby patří k jedné osobě (tedy jak je spojují do „kostry“).

PifPaf produkuje predikce přímo v obraze a spojování do osob probíhá až ve fázi dekódování, což je odlišné od top-down přístupů.

## Třetí přístup: Direct regression / anchor-based keypoints
Přímo regresuje souřadnice klíčových bodů (často podobně jako detektory objektů)

Typicky to vypadá jako:
- síť najde objekt (pes / tělo)
- současně predikuje:
- bounding box
- rovnou (x,y) pozice kloubů

Vlastnosti:

✅ rychlé
✅ jednoduchý pipeline
❌ obvykle méně přesné než heatmapy
❌ hůř se učí jemné detaily

Používá se často v realtime systémech (mobil, embedded).
