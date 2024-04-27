# Curs de LaTeX (enfocat a la lingüística)

Diapositives per a un curs d'introducció a LaTeX. Les diapositives i el codi es basen en
[aquest repositori de github](https://github.com/jdleesmiller/latex-course) sota una llicència permissiva
del MIT.

L'objectiu és que els estudiants escriguin a LaTeX el més ràpidament possible. El material es presenta
com un conjunt d'exemples, i a mesura que van sorgint s'expliquen conceptes i tècniques més àmplies. Cada
part inclou exercicis que es poden completar a [Overleaf](https://www.overleaf.com), l'editor LaTeX
gratuït en línia, de manera que no us haureu de preocupar d'instal·lar LaTeX i eines relacionades als
ordinadors de tothom.

1. [The Basics](http://jdleesmiller.github.io/latex-course/en/part1.pdf): ideas, syntax, equations,
   environments, packages

1. [Structed Documents & More](http://jdleesmiller.github.io/latex-course/en/part2.pdf): titles,
   sections, cross-references, figures, tables, bibliographies.

1. [Not Just Papers: Presentations & More](http://jdleesmiller.github.io/latex-course/en/part3.pdf):
   recap exercise, presentations with beamer, drawings with tikz.

## Compilació

Calen alguns paquets extres per compilar-ho en local.

1. [minted](http://www.ctan.org/pkg/minted) per la sintaxi en colors, ve amb les versions més recents
   de TeX Live.

2. [pygments](http://pygments.org/): `sudo apt-get install python-pygments`

1. `make` per fer servir el `Makefile`.

Les diapositives inclouen enllaços a exercicis que s'obren a Overleaf, però els fitxers es troben
a aquest repositori.
