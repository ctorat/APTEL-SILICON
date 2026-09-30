#
# Copyright (c) 2026, Apollo Telephone Laboratories.
# Provided under the BSD-3 clause.
#

TYPST_FILES = $(shell find src/ -name "*.typ")
PDF_FILES = $(TYPST_FILES:.typ=.pdf)

.PHONY: all
all: $(PDF_FILES)
	mv $(PDF_FILES) .

%.pdf: %.typ
	typst compile $<
