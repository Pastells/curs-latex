all: part1.pdf part2.pdf part3.pdf recap.pdf

#
# Part 1
#
part1.pdf: part1.tex preamble.tex media-graphics.pdf media-tables.pdf
	pdflatex -shell-escape part1
	pdflatex -shell-escape part1

media-graphics.pdf: media-graphics.tex
	lualatex media-graphics
	lualatex media-graphics

media-tables.pdf: media-tables.tex
	pdflatex media-tables
	pdflatex media-tables

#
# Part 2
#
part2.pdf: part2.tex preamble.tex structure-title.pdf structure-sections.pdf structure-sections-toc.pdf structure-crossref.pdf structure-cleveref.pdf bib-example.pdf structure-exercise-solution.pdf media-graphics-tables.pdf recap-structure.pdf recap-exercise.pdf recap-exercise-solution.pdf
	pdflatex -shell-escape part2
	pdflatex -shell-escape part2

structure-title.pdf: structure-title.tex
	pdflatex structure-title

structure-sections.pdf: structure-sections.tex
	pdflatex structure-sections

structure-sections-toc.pdf: structure-sections-toc.tex
	pdflatex structure-sections-toc

structure-crossref.pdf: structure-crossref.tex
	pdflatex structure-crossref
	pdflatex structure-crossref

structure-cleveref.pdf: structure-cleveref.tex 
	pdflatex structure-cleveref
	pdflatex structure-cleveref

structure-exercise-solution.pdf: structure-exercise-solution.tex
	pdflatex structure-exercise-solution
	pdflatex structure-exercise-solution
	pdflatex structure-exercise-solution


bib-example.pdf: bib-example.tex bib-example.bib
	pdflatex bib-example
	biber bib-example
	pdflatex bib-example
	pdflatex bib-example

#
# Recap 
#
recap.pdf: recap.tex preamble.tex media-graphics-tables.pdf recap-structure.pdf recap-exercise.pdf recap-exercise-solution.pdf
	pdflatex -shell-escape recap
	pdflatex -shell-escape recap

media-graphics-tables.pdf: media-graphics-tables.tex
	pdflatex media-graphics-tables
	pdflatex media-graphics-tables

recap-structure.pdf: recap-structure.tex
	pdflatex recap-structure

recap-exercise.pdf: recap-exercise.tex
	pdflatex recap-exercise

recap-exercise-solution.pdf: recap-exercise-solution.tex
	pdflatex recap-exercise-solution

#
# Part 3
#
part3.pdf: part3.tex preamble.tex ipa.pdf ipa-vowel.pdf beamer-minimal.pdf beamer-theme.pdf beamer-exercise.pdf beamer-exercise-solution.pdf
	pdflatex -shell-escape part3
	pdflatex -shell-escape part3

ipa.pdf: ipa.tex
	lualatex ipa 

ipa-vowel.pdf: ipa-vowel.tex
	lualatex ipa-vowel 

beamer-minimal.pdf: beamer-minimal.tex
	pdflatex beamer-minimal

beamer-theme.pdf: beamer-theme.tex
	pdflatex beamer-theme

beamer-exercise.pdf: beamer-exercise.tex
	pdflatex beamer-exercise

beamer-exercise-solution.pdf: beamer-exercise-solution.tex
	pdflatex beamer-exercise-solution
	pdflatex beamer-exercise-solution

latex-course.tgz: part1.pdf part2.pdf part3.pdf basics-exercise-1-solution.tex basics-exercise-1.tex basics-exercise-2-solution.tex basics-exercise-2.tex basics.tex bib-example.tex preamble.tex structure-exercise-solution.tex structure-exercise-solution.pdf structure-exercise.tex gus.png gus_gran.png khaleesi.jpg khaleesi2.jpg bib-exercise.bib recap-exercise.tex recap-exercise-solution.pdf beamer-minimal.tex beamer-exercise.tex beamer-exercise-solution.pdf gettysburg_graph.png
	tar czf latex-course.tgz $^

clean:
	rm -f *.log *.aux *.out *.nav *.snm *.toc *.vrb *.pyg *.bbl *.blg structure-crossref.pdf structure-sections.pdf structure-title.pdf media-graphics.pdf media-tables.pdf bib-example.pdf

clobber: clean
	rm -f part1.pdf part2.pdf part3.pdf
