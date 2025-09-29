# Dossiers
CODE := $(shell pwd)
PDFDIR = ../../pdf/3eme
THEME = 

# Visualiser les pdf
LOG=evince

# Créer le dossier pdf s'il n'éxiste pas.
target:
	test -d $(PDFDIR) || mkdir $(PDFDIR)

all: img poly proper

# Générations des images
FIGSRC = $(wildcard 4x7-triangles-semblables/*.ipe 4x3-triangles-semblables/*.ipe 4x1-pythagore/*.ipe 4x8-pythagore-2/*.ipe 4xbb/*.ipe 4x14-trigonometrie/*.ipe 4xDM/*.ipe)

FIGOBJ = $(FIGSRC:.ipe=.pdf)

img: $(FIGOBJ)

4x3-triangles-semblables/%.pdf: 4x3-triangles-semblables/%.ipe
	ipetoipe -pdf $<

4x1-pythagore/%.pdf: 4x1-pythagore/%.ipe
	ipetoipe -pdf $<


4x8-pythagore-2/%.pdf: 4x8-pythagore-2/%.ipe
	ipetoipe -pdf $<

4x14-trigonometrie/%.pdf: 4x14-trigonometrie/%.ipe
	ipetoipe -pdf $<

4xDM/%.pdf: 4xDM/%.ipe
	ipetoipe -pdf $<

4x7-triangles-semblables/%.pdf: 4x7-triangles-semblables/%.ipe
	ipetoipe -pdf $<

1py:
	pdflatex 4x1-pythagore/4x1-pythagore.tex
	pdflatex 4x1-pythagore/4x1-pythagore.tex
	mv 4x1-pythagore.pdf '$(PDFDIR)'/4x1-pythagore.pdf

1exo1:
	pdflatex 4x1-pythagore/4x1-exo1.tex
	pdflatex 4x1-pythagore/4x1-exo1.tex
	mv 4x1-exo1.pdf '$(PDFDIR)'/4x1-exo1.pdf

1exo2:
	pdflatex 4x1-pythagore/4x1-exo2.tex
	pdflatex 4x1-pythagore/4x1-exo2.tex
	mv 4x1-exo2.pdf '$(PDFDIR)'/4x1-exo2.pdf

DM1:
	pdflatex 4xDM/4x1-DM.tex
	pdflatex 4xDM/4x1-DM.tex
	mv 4x1-DM.pdf '$(PDFDIR)'/4x1-DM.pdf

1ie:
	pdflatex 3x1-calcul-litteral/3x1-ie.tex
	pdflatex 3x1-calcul-litteral/3x1-ie.tex
	mv 3x1-ie.pdf '$(PDFDIR)'/3x1-ie.pdf

DM2:
	pdflatex 4xDM/4x2-DM.tex
	pdflatex 4xDM/4x2-DM.tex
	mv 4x2-DM.pdf '$(PDFDIR)'/4x2-DM.pdf

2ie:
	pdflatex 4x2-nombres-relatifs/4x2-ie.tex
	pdflatex 4x2-nombres-relatifs/4x2-ie.tex
	mv 4x2-ie.pdf '$(PDFDIR)'/4x2-ie.pdf


2data:
	pdflatex 4x2-graphiques/4x2-data-perso.tex
	pdflatex 4x2-graphiques/4x2-data-perso.tex
	mv 4x2-data-perso.pdf '$(PDFDIR)'/4x2-data-perso.pdf
	pdflatex 4x2-graphiques/4x2-data-temperature.tex
	pdflatex 4x2-graphiques/4x2-data-temperature.tex
	mv 4x2-data-temperature.pdf '$(PDFDIR)'/4x2-data-temperature.pdf

3ie:
	pdflatex 4x3-proportionnalite/4x3-ie.tex
	pdflatex 4x3-proportionnalite/4x3-ie.tex
	mv 4x3-ie.pdf '$(PDFDIR)'/4x3-ie-prop.pdf

4ie:
	pdflatex 4x4-educfi/4x4-ie.tex
	pdflatex 4x4-educfi/4x4-ie.tex
	mv 4x4-ie.pdf '$(PDFDIR)'/4x4-ie-educfi.pdf


sem1:
	pdflatex 4xDM/4x-sem1.tex
	pdflatex 4xDM/4x-sem1.tex
	mv 4x-sem1.pdf '$(PDFDIR)'/4x-sem1.pdf


5exo1:
	pdflatex 4x5-puissances/4x5-exo-1.tex
	pdflatex 4x5-puissances/4x5-exo-1.tex
	mv 4x5-exo-1.pdf '$(PDFDIR)'/4x5-exo-1.pdf



5exo2:
	pdflatex 4x5-puissances/4x5-exo-2.tex
	pdflatex 4x5-puissances/4x5-exo-2.tex
	mv 4x5-exo-2.pdf '$(PDFDIR)'/4x5-exo-2.pdf

5ie:
	pdflatex 4x5-puissances/4x5-ie.tex
	pdflatex 4x5-puissances/4x5-ie.tex
	mv 4x5-ie.pdf '$(PDFDIR)'/4x5-ie.pdf

5dm:
	pdflatex 4xDM/4x3-DM.tex
	pdflatex 4xDM/4x3-DM.tex
	mv 4x3-DM.pdf '$(PDFDIR)'/4x3-DM.pdf


6ie:
	pdflatex 4x6-notation-scientifique/4x6-ie.tex
	pdflatex 4x6-notation-scientifique/4x6-ie.tex
	mv 4x6-ie.pdf '$(PDFDIR)'/4x6-ie-sci.pdf	


7ie:
	pdflatex 4x7-triangles-semblables/4x7-ie.tex
	pdflatex 4x7-triangles-semblables/4x7-ie.tex
	mv 4x7-ie.pdf '$(PDFDIR)'/4x7-ie.pdf	


14dm:
	pdflatex 4x14-trigonometrie/4x14-dm.tex
	pdflatex 4x14-trigonometrie/4x14-dm.tex
	mv 4x14-dm.pdf '$(PDFDIR)'/4x14-dm-trigo.pdf	
	
14ie:
	pdflatex 4x14-trigonometrie/4x14-ie.tex
	pdflatex 4x14-trigonometrie/4x14-ie.tex
	mv 4x14-ie.pdf '$(PDFDIR)'/4x14-ie-trigo.pdf	


# nettoyage		
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi *.ps
	rm -f *.backup *~
