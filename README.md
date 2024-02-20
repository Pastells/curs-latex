# latex-course

Diapositives per a un curs d'introducció a LaTeX. Les diapositives i el codi es basen en el
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

## Development

You may need to install some extra LaTeX packages and system packages in order to build the slides
yourself.

1. The [minted package](http://www.ctan.org/pkg/minted) provides syntax highlighting. It is installed by
   default in recent versions of TeX Live.

1. The minted package calls out to the [pygments syntax highlighter](http://pygments.org/), which is
   written in python. The relevant package is python-pygments in Debian / Ubuntu
   (`sudo apt-get install python-pygments`).

1. There is a simple `Makefile` that manages the build. To use it, you'll probably need to be on Linux,
   and you will need `make`.

The slides include links to exercises that open in Overleaf. The exercise source files are hosted on
github. If you want to use exercise files in another location, you can
[fork](https://help.github.com/articles/fork-a-repo) this github repository and then change the
`\fileuri` macro in `preamble.tex`:

```
\newcommand{\fileuri}{https://raw.github.com/jdleesmiller/latex-course/master/en}
```

so that instead of pointing to `jdleesmiller/latex-course`, it points to
`your-github-user-name/latex-course`. Then, once you've pushed your changed exercise files to github, the
slides will load them up in Overleaf.

The `deploy-to-gh-pages.sh` script builds the slides using the Makefile and copies the slides over to the
`gh-pages` branch, which is available at `http://jdlm.info/latex-course` thanks to
[github pages](http://pages.github.com/).

## License

The slides and source are released under the MIT license. See the LICENSE file.
