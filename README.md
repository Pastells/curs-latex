# Curs de LaTeX (enfocat a la lingüística)

Diapositives per a un curs d'introducció a LaTeX. Les diapositives i el codi es basen en
[aquest repositori de github](https://github.com/jdleesmiller/latex-course) sota una llicència permissiva
del MIT.

L'objectiu és que els estudiants escriguin amb LaTeX el més ràpidament possible. El material es presenta
com un conjunt d'exemples, i a mesura que van sorgint s'expliquen conceptes i tècniques més àmplies. Cada
part inclou exercicis que es poden completar a [Overleaf](https://www.overleaf.com), l'editor LaTeX
gratuït en línia, de manera que no us haureu de preocupar d'instal·lar LaTeX i eines relacionades.

El material està dividit en 3 classes de dues hores:

1. [Primera part](https://github.com/Pastells/curs-latex/blob/master/ca/part1.pdf):
   Sintaxi, entorns, paquets, figures i taules

2. [Segona part](https://github.com/Pastells/curs-latex/blob/master/ca/part2.pdf) (EN PROCÉS):
   Seccions, referències creuades, bibliografia, paquets lingüística (`linguex` i `tipa`).

2.5. [Repàs](https://github.com/Pastells/curs-latex/blob/master/ca/recap.pdf)

3. [Tercera part](https://github.com/Pastells/curs-latex/blob/master/ca/part3.pdf) (EN PROCÉS):
   Notes i comentaris, presentacions amb `beamer`.

## Compilació

Calen alguns paquets extres per compilar-ho en local.

1. [minted](http://www.ctan.org/pkg/minted) per la sintaxi en colors, ve amb les versions més recents
   de TeX Live.

2. [pygments](http://pygments.org/): `sudo apt-get install python-pygments`

1. `make` per fer servir el `Makefile`.

Les diapositives inclouen enllaços a exercicis que s'obren a Overleaf, però els fitxers es troben
a aquest repositori.
