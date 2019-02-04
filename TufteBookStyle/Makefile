MODE = batchmode
TEX = pdflatex -synctex=1 -interaction=$(MODE)
MKINDEX = makeindex
BIBER = biber

SCRIPTFILE = Script.tex
DEFINITIONSFILE = Definitions.tex
FILES = $(SCRIPTFILE) $(DEFINITIONSFILE)

%.pdf: %.tex
	$(TEX) $<

.PHONY: index
.PHONY: bib
index: Script.pdf
	$(MKINDEX) Script.idx

bib: Script.pdf
	$(BIBER) Script.bcf
Script.pdf: $(FILES)
