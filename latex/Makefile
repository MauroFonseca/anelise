# Compilar todas las aulas y el informe de mejoras
# Requisito: tener `tectonic` instalado (https://tectonic-typesetting.github.io)
#   brew install tectonic   (macOS)

AULAS  = aula1 aula2 aula3 aula4 aula5 aula6
PDFS   = $(AULAS:=.pdf) informe_melloras.pdf

all: $(PDFS)

%.pdf: %.tex preamble.tex
	tectonic -X compile --keep-intermediates $*.tex

informe_melloras.pdf: inform ../docs/informe_melloras.tex
	tectonic -X compile --keep-intermediates ../docs/informe_melloras.tex

clean:
	rm -f *.aux *.log *.nav *.toc *.out *.xdv *.fdb_latexmk

cleanall: clean
	rm -f *.pdf

.PHONY: all clean cleanall inform