.PHONY: presentation.pdf all watch clean

all: presentation.pdf

presentation.pdf: presentation.tex
	latexmk -lualatex -use-make -f -quiet -interaction=nonstopmode $(PREVIEW_CONTINUOUSLY) presentation.tex

watch: PREVIEW_CONTINUOUSLY=-pvc -view=none
watch: presentation.pdf

clean:
	latexmk -CA
