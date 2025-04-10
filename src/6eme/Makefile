# Dossiers
CODE := $(shell pwd)
PDFDIR = ../../pdf/6eme
THEME = 

# Visualiser les pdf
LOG=evince

# Créer le dossier pdf s'il n'éxiste pas.
target:
	test -d $(PDFDIR) || mkdir $(PDFDIR)

all: img poly proper

# Générations des images
FIGSRC = $(wildcard 6x1-fractions/*.ipe 6x2-geometrie-quadrillage/*.ipe 6x4-symetrie/*.ipe 4xbb/*.ipe 6x4-geometrie-base/*.ipe 6x7-aires-perimetres/*.ipe)

FIGOBJ = $(FIGSRC:.ipe=.pdf)

img: $(FIGOBJ)

6x1-fractions/%.pdf: 6x1-fractions/%.ipe
	ipetoipe -pdf $<

6x4-symetrie/%.pdf: 6x4-symetrie/%.ipe
	ipetoipe -pdf $<

6x2-geometrie-quadrillage/%.pdf: 6x2-geometrie-quadrillage/%.ipe
	ipetoipe -pdf $<

6x4-geometrie-base/%.pdf: 6x4-geometrie-base/%.ipe
	ipetoipe -pdf $<

6x7-aires-perimetres/%.pdf: 6x7-aires-perimetres/%.ipe
	ipetoipe -pdf $<	

1cours:
	pdflatex 6x1-fractions/6x1-fractions.tex
	pdflatex 6x1-fractions/6x1-fractions.tex
	mv 6x1-fractions.pdf '$(PDFDIR)'/6x1-fractions.pdf

1ie:
	pdflatex 6x1-fractions/6x1-ie.tex
	pdflatex 6x1-fractions/6x1-ie.tex
	mv 6x1-ie.pdf '$(PDFDIR)'/6x1-ie.pdf

DM1:
	pdflatex 6xDM/6x1-DM.tex
	pdflatex 6xDM/6x1-DM.tex
	mv 6x1-DM.pdf '$(PDFDIR)'/6x1-DM.pdf

2ie:
	pdflatex 6x2-geometrie-quadrillage/6x2-ie.tex
	pdflatex 6x2-geometrie-quadrillage/6x2-ie.tex
	mv 6x2-ie.pdf '$(PDFDIR)'/6x2-ie.pdf

3ie:
	pdflatex 6x3-fractions-2/6x3-ie.tex
	pdflatex 6x3-fractions-2/6x3-ie.tex
	mv 6x3-ie.pdf '$(PDFDIR)'/6x3-ie.pdf

4ie:
	pdflatex 6x4-symetrie/6x4-ie.tex
	pdflatex 6x4-symetrie/6x4-ie.tex
	mv 6x4-ie.pdf '$(PDFDIR)'/6x4-ie.pdf

5ie:
	pdflatex 6x5-fractions-3/6x5-ie.tex
	pdflatex 6x5-fractions-3/6x5-ie.tex
	mv 6x5-ie.pdf '$(PDFDIR)'/6x5-ie.pdf

6ie:
	pdflatex 6x6-calculs-geo/6x6-ie.tex
	pdflatex 6x6-calculs-geo/6x6-ie.tex
	mv 6x6-ie.pdf '$(PDFDIR)'/6x6-ie.pdf

7ie:
	pdflatex 6x7-aires-perimetres/6x7-ie.tex
	pdflatex 6x7-aires-perimetres/6x7-ie.tex
	mv 6x7-ie.pdf '$(PDFDIR)'/6x7-ie.pdf

8ie:
	pdflatex 6x8-nombres-entiers/6x8-ie.tex
	pdflatex 6x8-nombres-entiers/6x8-ie.tex
	mv 6x8-ie.pdf '$(PDFDIR)'/6x8-ie.pdf

8dm:
	pdflatex 6x8-temps/6x8-dm.tex
	pdflatex 6x8-temps/6x8-dm.tex
	mv 6x8-dm.pdf '$(PDFDIR)'/6x8-dm.pdf

# nettoyage		
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi *.ps
	rm -f *.backup *~
