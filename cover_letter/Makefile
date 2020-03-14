.PHONY : all latex bibtex pdf view clean distclean

TARGET=cl_aloise
SOURCE=$(TARGET).tex
SUPPLEMENTARY_TARGET=supplementary_material
SUPPLEMENTARY_SOURCE=$(SUPPLEMENTARY_TARGET).tex

all:
	pdflatex $(SOURCE)
# bibtex $(TARGET)
	pdflatex $(SOURCE)
	pdflatex $(SOURCE)
#	pdflatex $(SUPPLEMENTARY_SOURCE)
#	pdflatex $(SUPPLEMENTARY_SOURCE)

latex:
	pdflatex $(SOURCE)
	pdflatex $(SOURCE)
#	pdflatex $(SUPPLEMENTARY_SOURCE)
#	pdflatex $(SUPPLEMENTARY_SOURCE)

bibtex:
	bibtex $(TARGET)

view:
	open $(TARGET).pdf &

clean:
	rm -f $(TARGET).aux $(TARGET).bbl $(TARGET).blg $(TARGET).log $(TARGET).brf $(TARGET).synctex.gz $(TARGET).out $(TARGET).glo $(TARGET).ist $(TARGET).gls $(TARGET).glg
# rm -f $(SUPPLEMENTARY_TARGET).aux $(SUPPLEMENTARY_TARGET).bbl $(SUPPLEMENTARY_TARGET).blg $(SUPPLEMENTARY_TARGET).log $(SUPPLEMENTARY_TARGET).brf $(SUPPLEMENTARY_TARGET).synctex.gz $(SUPPLEMENTARY_TARGET).out $(SUPPLEMENTARY_TARGET).glo $(SUPPLEMENTARY_TARGET).ist $(SUPPLEMENTARY_TARGET).gls $(SUPPLEMENTARY_TARGET).glg

distclean:clean
	rm -f $(TARGET).pdf
#	rm -f $(SUPPLEMENTARY_TARGET).pdf
