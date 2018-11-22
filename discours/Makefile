DEP := $(shell find . -name "*.tex") 

MAIN = main
CIBLE = compilation/$(MAIN).pdf


$(CIBLE) : $(DEP)
	rm -f compilation/$(MAIN).glo compilation/$(MAIN).glsdefs
	latexmk -pdf -output-directory=compilation $(MAIN).tex

clean :
	@rm -f *.aux *~ *.bbl *.blg *.glg *.glo *.gls *.ist *.log 

.PHONY: $(CIBLE)
