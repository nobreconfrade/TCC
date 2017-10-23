.PHONY: main
main:
	pdflatex main
	bibtex main
	pdflatex main
	pdflatex main


.PHONY: x
x:
	xelatex -interaction=nonstopmode main
	bibtex main
	xelatex -interaction=nonstopmode main
	xelatex -interaction=nonstopmode main

.PHONY: clean
clean:
	rm -f *.log *.dvi *.lof *.lot *.nlo *.out *.toc *.aux *.bak *.bbl *.blg *.gz *.fdb_latexmk *.fls *.log *.synctex.gz

.PHONY: view
view: main
	open main.pdf
