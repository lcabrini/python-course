COMMON_DIR = /usr/local/training-materials-common
ASCIIDOCTOR = asciidoctor-pdf
WORKBOOK = python-001-workbook.pdf
PRESENTATION = python-001-presentation.pdf
PDF = $(WORKBOOK) $(PRESENTATION)
THEME = -a pdf-style=$(COMMON_DIR)/theme/presentation-theme.yml

all: $(PDF)

$(WORKBOOK): workbook.adoc
	$(ASCIIDOCTOR) workbook.adoc -o $@

$(PRESENTATION): presentation.adoc
	$(ASCIIDOCTOR) presentation.adoc $(THEME) -o $@

clean:
	$(RM) $(PDF)
