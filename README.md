2D-Point-Localization

## Zadání:
- Implementace algoritmu pro rychlé hledání bodu v rovině.
- Vytvoření datové struktury pro předzpracování roviny.

## Algoritmus:
### Předzpracování:
1. Načteme rovinu. (Předpokládáme, že rovina je Voronův diagram nebo rovinný graf uzavřený na polygony.)
2. Seřadíme body podle Y souřadnice.
3. Vytvoříme n-1 pásů z dvojic bodů jdoucích za sebou. (Předpokládáme že každá Y souřadnice je unikátní. Když není, tak celou rovinu trošku pootočíme, smažeme pásy a vrátíme se k bodu 2.)
4. Postupně projdeme všechny body odzhora dolů a pro každý bod B:
- 5. Odstraníme hrany vedoucí směřem nad bod B.