# Ideový plán: ForgeAim

## Formální Název projektu
**ForgeAim** *(Případně: CoreAim / ReflexTrainer)*

## Marketingový úvodník
Posuň své mechanické limity na maximum. ForgeAim je ultimátní tréninkový nástroj navržený pro hráče taktických FPS her, kteří chtějí dominovat v duelech. Ať už potřebuješ zahřát zápěstí před rankedem, nebo dlouhodobě trénovat micro-adjustments a tracking, ForgeAim ti poskytne čisté, plynulé a analytické prostředí, kde se každé kliknutí počítá. Trénuj chytřeji, trefuj rychleji.

## Popis hry
**Principy:** 
Hra je založena na rychlém a přesném ničení dynamicky se objevujících cílů (terčů/koulí) ve 3D prostoru z pohledu první osoby. 

**Funkčnost a možnosti (Herní režimy):**
*   **Gridshot/Flicking:** Rychlé přepínání mezi statickými terči s důrazem na hrubou rychlost a svalovou paměť.
*   **Tracking:** Udržení zaměřovače na plynule se pohybujícím terči s nepredikovatelnými změnami směru.
*   **Micro-adjustments:** Drobné, extrémně přesné pohyby na malé a vzdálené terče (simulace střelby na hlavu na velkou vzdálenost).
*   **Analytika:** Po každém scénáři hráč vidí své statistiky (přesnost v %, reakční doba v ms, skóre).

**Cíle hráče:**
Cílem hráče je překonávat svá osobní maxima (High Scores), udržovat konzistentní přesnost (ideálně nad 90 %) a analyzovat svůj progres v čase, aby tyto dovednosti přenesl do svých hlavních her.

## Popis audiovizuálu
**Vizuál:** Striktně minimalistický a funkční. Cílem je nulová vizuální latence a maximální čitelnost. Prostředí (stěny, podlaha) bude v tmavě šedých nebo neutrálních texturách bez rušivých elementů. Terče budou využívat vysoce kontrastní neonové barvy (např. tyrkysová, magenta, jasně žlutá), aby okamžitě upoutaly periferní vidění. 
**Audio:** Ostrá, uspokojující zvuková odezva (hit sound) při každém úspěšném zničení terče, která psychologicky odměňuje hráče. Žádná rušivá hudba během tréninku.

## Chystané použité technologie
*   **Herní Engine:** Unity (využití jazyka C# pro skriptování herní logiky a pohybu terčů) *nebo* Godot.
*   **Verzování:** Git a GitHub.
*   **Ukládání dat:** Lokální JSON soubory nebo jednoduchá SQLite databáze pro ukládání historie hráčových statistik a high scores.

## Hypotézy (k potvrzení/vyvrácení po releasu)
1. **Hypotéza o náročnosti režimů:** Z dostupných herních režimů bude nejnáročnější režim "Micro-adjustments". Očekávám, že v tomto režimu dosáhnou hráči plošně nejnižší průměrné přesnosti (accuracy) ve srovnání s režimem "Gridshot", protože vyžaduje mnohem jemnější motoriku myši, na kterou běžní uživatelé nejsou zvyklí.
2. **Hypotéza Časovém stresu a zmatkování:** Většině testujících se v posledních 10 vteřinách limitu (kdy uvidí, že jim dochází čas) radikálně sníží přesnost střelby oproti první polovině hry, protože přestanou pečlivě mířit a začnou panicky klikat.
