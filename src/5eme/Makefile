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

2cours:
	pdflatex 5x2-probabilite/5x2-cours.tex
	pdflatex 5x2-probabilite/5x2-cours.tex
	mv 5x2-cours.pdf '$(PDFDIR)'/5x2-cours.pdf

2ie:
	pdflatex 5x2-probabilite/5x2-ie.tex
	pdflatex 5x2-probabilite/5x2-ie.tex
	mv 5x2-ie.pdf '$(PDFDIR)'/5x2-ie.pdf

3cours:
	pdflatex 5x3-nombres-relatifs-1-intro/5x3-cours.tex
	pdflatex 5x3-nombres-relatifs-1-intro/5x3-cours.tex
	mv 5x3-cours.pdf '$(PDFDIR)'/5x3-cours.pdf

3ie:
	pdflatex 5x3-nombres-relatifs-1-intro/5x3-ie.tex
	pdflatex 5x3-nombres-relatifs-1-intro/5x3-ie.tex
	mv 5x3-ie.pdf '$(PDFDIR)'/5x3-ie.pdf

4cours:
	pdflatex 5x4-symetrie-centrale-1-quadrillage/5x4-cours.tex
	pdflatex 5x4-symetrie-centrale-1-quadrillage/5x4-cours.tex
	mv 5x4-cours.pdf '$(PDFDIR)'/5x4-cours.pdf

4ie:
	pdflatex 5x4-symetrie-centrale-1-quadrillage/5x4-ie.tex
	pdflatex 5x4-symetrie-centrale-1-quadrillage/5x4-ie.tex
	mv 5x4-ie.pdf '$(PDFDIR)'/5x4-ie.pdf	


5cours:
	pdflatex 5x5-fractions-1-intro/5x5-cours.tex
	pdflatex 5x5-fractions-1-intro/5x5-cours.tex
	mv 5x5-cours.pdf '$(PDFDIR)'/5x5-cours.pdf

5ie:
	pdflatex 5x5-fractions-1-intro/5x5-ie.tex
	pdflatex 5x5-fractions-1-intro/5x5-ie.tex
	mv 5x5-ie.pdf '$(PDFDIR)'/5x5-ie.pdf

6cours:
	pdflatex 5x6-triangles-1-angles/5x6-cours.tex
	pdflatex 5x6-triangles-1-angles/5x6-cours.tex
	mv 5x6-cours.pdf '$(PDFDIR)'/5x6-cours.pdf

6dm:
	pdflatex 5x6-triangles-1-angles/5x6-dm.tex
	pdflatex 5x6-triangles-1-angles/5x6-dm.tex
	mv 5x6-dm.pdf '$(PDFDIR)'/5x6-dm.pdf

7cours:
	pdflatex 5x7-proportionnalite/5x7-cours.tex
	pdflatex 5x7-proportionnalite/5x7-cours.tex
	mv 5x7-cours.pdf '$(PDFDIR)'/5x7-cours.pdf

7ie:
	pdflatex 5x7-proportionnalite/5x7-ie.tex
	pdflatex 5x7-proportionnalite/5x7-ie.tex
	mv 5x7-ie.pdf '$(PDFDIR)'/5x7-ie.pdf


12exo1:
	pdflatex 5x12-calcul-litteral/5x12-exo1.tex
	pdflatex 5x12-calcul-litteral/5x12-exo1.tex
	mv 5x12-exo1.pdf '$(PDFDIR)'/5x12-exo1.pdf

12ie:
	pdflatex 5x12-calcul-litteral/5x12-ie.tex
	pdflatex 5x12-calcul-litteral/5x12-ie.tex
	mv 5x12-ie.pdf '$(PDFDIR)'/5x12-ie.pdf

17dm:
	pdflatex 5x17-pourcentages/5x17-dm.tex
	pdflatex 5x17-pourcentages/5x17-dm.tex
	mv 5x17-dm.pdf '$(PDFDIR)'/5x17-dm.pdf

18ie:
	pdflatex 5x18-triangles-2-inegalite-triangulaire/5x18-ie.tex
	pdflatex 5x18-triangles-2-inegalite-triangulaire/5x18-ie.tex
	mv 5x18-ie.pdf '$(PDFDIR)'/5x18-ie.pdf			

20ie:
	pdflatex 5x20-angles-et-parallelisme/5x20-ie.tex
	pdflatex 5x20-angles-et-parallelisme/5x20-ie.tex
	mv 5x20-ie.pdf '$(PDFDIR)'/5x20-ie.pdf			

# nettoyage		
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi *.ps
	rm -f *.backup *~
