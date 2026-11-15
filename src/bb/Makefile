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
	latex bb2-2025.tex
	dvips bb2-2025.dvi
	ps2pdf bb2-2025.ps
	mv bb2-2025.pdf '$(PDFDIR)'/bb2-2025-double.pdf


bbpro:
	pdflatex bb2-2025-pro.tex
	pdflatex bb2-2025-pro.tex
	mv bb2-2025-pro.pdf '$(PDFDIR)'/bb2-2025-pro.pdf


dm1:
	latex dm-1.tex
	dvips dm-1.dvi
	ps2pdf dm-1.ps
	mv dm-1.pdf '$(PDFDIR)'/dm-1.pdf


sante:
	pdflatex sante.tex
	pdflatex sante.tex
	mv sante.pdf '$(PDFDIR)'/sante.pdf

# nettoyage		
proper:
	rm -f *.log *.toc *.aux *.nav *.snm *.out *.bbl *.blg *.dvi *.ps
	rm -f *.backup *~
