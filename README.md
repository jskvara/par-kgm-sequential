# Úloha KGM: kostra grafu s minimálním stupněm

## Vstupní data:
G(V,E) = jednoduchý souvislý neorientovaný neohodnocený graf o n uzlech a m hranách

n = přirozené číslo představující počet uzlů grafu G, n >= 5
k = přirozené číslo řádu jednotek představující průměrný stupeň uzlu grafu G, n >= k >= 3

## Doporučení pro algoritmus generování G:
Použijte generátor grafu s volbou typu grafu „-t AD“, který vygeneruje souvislý neorientovaný neohodnocený graf.

## Definice:
Stupeň stromu je definován jako maximální stupeň ze všech uzlů stromu.

## Úkol:
Nalezněte kostru grafu G (strom) s minimálním stupněm.

## Výstup algoritmu:
Výpis kostry grafu G a hodnota stupně této kostry.

## Sekvenční algoritmus:
Řešení existuje vždy, vždy lze sestrojit kostru grafu. Sekvenční algoritmus je typu BB-DFS s hloubkou prohledávaného prostoru omezenou na |V|. Přípustný mezistav je definovaný částečnou kostrou. Přípustný koncový stav je vytvořená kostra. Algoritmus končí po prohledání celého prostoru či při dosažení dolní meze. Cena, kterou minimalizujeme, je stupeň kostry.

Těsná dolní mez je rovna 2.

Holní mez je rovna nejvyššímu stupni v grafu G.

## Paralelní algoritmus
Paralelní algoritmus je typu G-PBB-DFS-D.
