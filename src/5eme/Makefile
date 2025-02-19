# Dossiers
CODE := $(shell pwd)
PDFDIR = ../../pdf/5eme
THEME = 

# Visualiser les pdf
LOG=evince

# Créer le dossier pdf s'il n'éxiste pas.
target:
	test -d $(PDFDIR) || mkdir $(PDFDIR)

all: img poly proper

# Générations des images
FIGSRC = $(wildcard 5x1-calcul-numerique/*.ipe 5x3-nombres-relatifs-1-intro/*.ipe 5x4-symetrie-centrale-1-quadrillage/*.ipe 5x6-triangles-1-angles/*.ipe 4xbb/*.ipe 5x8-aires/*.ipe 5x20-angles-et-parallelisme/*.ipe)

FIGOBJ = $(FIGSRC:.ipe=.pdf)

img: $(FIGOBJ)

5x1-calcul-numerique/%.pdf: 5x1-calcul-numerique/%.ipe
	ipetoipe -pdf $<

5x3-nombres-relatifs-1-intro/%.pdf: 5x3-nombres-relatifs-1-intro/%.ipe
	ipetoipe -pdf $<

5x4-symetrie-centrale-1-quadrillage/%.pdf: 5x4-symetrie-centrale-1-quadrillage/%.ipe
	ipetoipe -pdf $<

5x6-triangles-1-angles/%.pdf: 5x6-triangles-1-angles/%.ipe
	ipetoipe -pdf $<

5x8-aires/%.pdf: 5x8-aires/%.ipe
	ipetoipe -pdf $<

5x20-angles-et-parallelisme/%.pdf: 5x20-angles-et-parallelisme/%.ipe
	ipetoipe -pdf $<


# Chapitre 1

1cours:
	pdflatex 5x1-calcul-numerique/5x1-cours.tex
	pdflatex 5x1-calcul-numerique/5x1-cours.tex
	mv 5x1-cours.pdf '$(PDFDIR)'/5x1-cours.pdf

1ie:
	pdflatex 5x1-calcul-numerique/5x1-ie.tex
	pdflatex 5x1-calcul-numerique/5x1-ie.tex
	mv 5x1-ie.pdf '$(PDFDIR)'/5x1-ie.pdf


DM1:
	pdflatex 5xDM/5x1-dm-apollo.tex
	pdflatex 5xDM/5x1-dm-apollo.tex
	mv 5x1-dm-apollo.pdf '$(PDFDIR)'/5x1-dm-apollo.pdf

1mini:
	pdflatex 5x1-calcul-numerique/5x1-mini.tex
	pdflatex 5x1-calcul-numerique/5x1-mini.tex
	mv 5x1-mini.pdf '$(PDFDIR)'/5x1-mini.pdf

2cours:
	pdflatex 5x2-probabilite/5x2-cours.tex
	pdflatex 5x2-probabilite/5x2-cours.tex
	mv 5x2-cours.pdf '$(PDFDIR)'/5x2-cours.pdf

2ie:
	pdflatex 5x2-inegalite-triangulaire/5x2-ie.tex
	pdflatex 5x2-inegalite-triangulaire/5x2-ie.tex
	mv 5x2-ie.pdf '$(PDFDIR)'/5x2-ie.pdf


DM2:
	pdflatex 5xDM/5x2-DM.tex
	pdflatex 5xDM/5x2-DM.tex
	mv 5x2-DM.pdf '$(PDFDIR)'/5x2-DM.pdf


3ie:
	pdflatex 5x3-tableau-proportionnel/5x3-ie.tex
	pdflatex 5x3-tableau-proportionnel/5x3-ie.tex
	mv 5x3-ie.pdf '$(PDFDIR)'/5x3-ie.pdf


4ie:
	pdflatex 5x4-statistiques/5x4-ie.tex
	pdflatex 5x4-statistiques/5x4-ie.tex
	mv 5x4-ie.pdf '$(PDFDIR)'/5x4-ie.pdf

5dm:
	pdflatex 5x5-equations/5x5-dm.tex
	pdflatex 5x5-equations/5x5-dm.tex
	mv 5x5-dm.pdf '$(PDFDIR)'/5x5-dm.pdf

5ie:
	pdflatex 5x5-equations/5x5-ie.tex
	pdflatex 5x5-equations/5x5-ie.tex
	mv 5x5-ie.pdf '$(PDFDIR)'/5x5-ie.pdf

# nettoyage		
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi *.ps
	rm -f *.backup *~
