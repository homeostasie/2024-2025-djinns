# Dossiers
CODE := $(shell pwd)
PDFDIR = ../../pdf/bb
THEME = 

# Visualiser les pdf
LOG=evince

# Créer le dossier pdf s'il n'éxiste pas.
target:
	test -d $(PDFDIR) || mkdir $(PDFDIR)


bb1:
	latex bb-2025.tex
	dvips bb-2025.dvi
	ps2pdf bb-2025.ps
	mv bb-2025.pdf '$(PDFDIR)'/bb-2025.pdf

bb1d:
	latex bb-2025-double.tex
	dvips bb-2025-double.dvi
	ps2pdf bb-2025-double.ps
	mv bb-2025-double.pdf '$(PDFDIR)'/bb-2025-double.pdf


bb2:
	pdflatex bb2-2025.tex
	pdflatex bb2-2025.tex
	mv bb2-2025.pdf '$(PDFDIR)'/bb2-2025-double.pdf

# nettoyage		
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi *.ps
	rm -f *.backup *~
