# Dossiers
CODE := $(shell pwd)
PDFDIR = ../../pdf/4eme
THEME = 

# Visualiser les pdf
LOG=evince

# Créer le dossier pdf s'il n'éxiste pas.
target:
	test -d $(PDFDIR) || mkdir $(PDFDIR)

all: img poly proper

# Générations des images
FIGSRC = $(wildcard 4x3-triangles-semblables/*.ipe 4x1-pythagore/*.ipe 4x8-pythagore-2/*.ipe 4xbb/*.ipe 4x14-trigonometrie/*.ipe)

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


1py:
	pdflatex 4x1-pythagore/4x1-pythagore.tex
	pdflatex 4x1-pythagore/4x1-pythagore.tex
	mv 4x1-pythagore.pdf '$(PDFDIR)'/4x1-pythagore.pdf

1exo:
	pdflatex 4x1-pythagore/4x1-exo.tex
	pdflatex 4x1-pythagore/4x1-exo.tex
	mv 4x1-exo.pdf '$(PDFDIR)'/4x1-exo.pdf

DM1:
	pdflatex 4xDM/4x1-DM.tex
	pdflatex 4xDM/4x1-DM.tex
	mv 4x1-DM.pdf '$(PDFDIR)'/4x1-DM.pdf
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

6ie:
	pdflatex 4x6-notation-scientifique/4x6-ie.tex
	pdflatex 4x6-notation-scientifique/4x6-ie.tex
	mv 4x6-ie.pdf '$(PDFDIR)'/4x6-ie-sci.pdf	


7dm:
	pdflatex 4x7-pythagore-1/4x7-dm.tex
	pdflatex 4x7-pythagore-1/4x7-dm.tex
	mv 4x7-dm.pdf '$(PDFDIR)'/4x7-dm-pytha.pdf	


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
