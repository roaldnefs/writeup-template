# Makefile

SOURCE_DOCS := $(wildcard *.md)
EXPORTED_DOCS=\
  $(SOURCE_DOCS:.md=.pdf)

RM=/bin/rm

PANDOC=/usr/local/bin/pandoc

PANDOC_OPTIONS=--from markdown --template eisvogel --listings

PANDOC_PDF_OPTIONS=

%.pdf : %.md
		$(PANDOC) $(PANDOC_OPTIONS) $(PANDOC_PDF_OPTIONS) -o $@ $<

.PHONY: all clean

all: $(EXPORTED_DOCS)

clean:
		- $(RM) $(EXPORTED_DOCS)