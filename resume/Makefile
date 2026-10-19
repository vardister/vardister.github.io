TEX_FILE := resume.tex
PDF_FILE := resume.pdf
SITE_PDF := ../files/resume_industry.pdf

.PHONY: build copy clean ci

build:
	latexmk -pdf -interaction=nonstopmode -halt-on-error $(TEX_FILE)

copy: build
	cp $(PDF_FILE) $(SITE_PDF)

ci: copy

clean:
	latexmk -C
	rm -f $(PDF_FILE)
