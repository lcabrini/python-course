ASCIIDOCTOR = asciidoctor-pdf
PDF = python-001-workbook.pdf python-001-presentation.pdf
THEME = -a pdf-style=../theme/presentation-theme.yml

all: $(PDF)

python-001-workbook.pdf: workbook.adoc
	asciidoctor-pdf workbook.adoc -o $@

python-001-presentation.pdf: presentation.adoc
	asciidoctor-pdf presentation.adoc $(THEME) -o $@

clean:
	$(RM) $(PDF)
