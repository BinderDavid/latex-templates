MODE = batchmode
LATEX = pdflatex -interactionmode=$(MODE)

presentation: presentation.tex
	$(LATEX) presentation.tex

.PHONY: view
view: presentation.pdf
	xdg-open presentation.pdf
