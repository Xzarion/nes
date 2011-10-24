SHELL := bash

FILES  = Protocol.tex highlevel-application.tex
FILES += ProtocolHeader.sty Makefile
TARGET = nesspecc.pdf

PDFGEN = pdflatex --jobname=$(basename $@) $<

all: $(TARGET)

$(TARGET): $(FILES)
	$(PDFGEN)
	$(PDFGEN)
	$(PDFGEN)



.PHONY: clean html

clean:
	rm -fr *.aux *.log *.dvi *.pdf *.toc *.out *.o testpcc

CC := gcc
#ppc environment only...
testppc: ppc.o testppc.o
	$(CC) -o $@ $^
