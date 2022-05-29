all: pdf clean

pdf:
	pdflatex main.tex
	bibtex refs.bib
	pdflatex main.tex

texmk: 
	latexmk -bibtex -xelatex \
	-synctex=1 main.tex

bib:
	bibtex8 -B -c utf8cyrillic.csf main.aux
clean:
	del -fr *.aux
	del -fr *.bbl
	del -fr *.blg
	del -fr *.log
	del -fr *.out
	del -fr *.toc
	del -fr *.dvi
	del -fr *.fls
	del -fr *.fdb_latexmk
	del -fr *.synctex.gz
	del -fr *.xdv
