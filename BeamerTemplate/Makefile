MODE = batchmode
LATEX = pdflatex -interactionmode=$(MODE)

presentation: presentation.tex
	$(LATEX) presentation.tex

.PHONY: view
view: presentation.pdf
	xdg-open presentation.pdf

.PHONY: clean
clean:
	rm *.nav
	rm *.aux
	rm *.out
	rm *.log
	rm *.snm
	rm *.toc
	rm *.pdf
