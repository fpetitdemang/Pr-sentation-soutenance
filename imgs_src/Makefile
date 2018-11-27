
all: ../imgs/dev_evolutionnaire.pdf ../imgs/slide_intro_process.pdf 

 
../imgs/dev_evolutionnaire.pdf : dev_evolutionnaire.tex
	latexmk -pdf -output-directory=../compilation dev_evolutionnaire.tex
	mv ../compilation/dev_evolutionnaire.pdf ../imgs

../imgs/slide_intro_process.pdf : slide_intro_process.tex
	latexmk -pdf -output-directory=../compilation slide_intro_process.tex
	mv ../compilation/slide_intro_process.pdf ../imgs

clean :
	@rm -f *.aux *~ *.bbl *.blg *.glg *.glo *.gls *.ist *.log 

.PHONY: $(CIBLE)
