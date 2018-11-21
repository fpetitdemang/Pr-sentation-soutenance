
all: ../imgs/slide_intro_pb_reconf.pdf ../imgs/logiciel.pdf ../imgs/slide_intro_process.pdf 

 
../imgs/slide_intro_pb_reconf.pdf : slide_intro_pb_reconf.tex
	latexmk -pdf -output-directory=../compilation slide_intro_pb_reconf.tex
	mv ../compilation/slide_intro_pb_reconf.pdf ../imgs

../imgs/logiciel.pdf : logiciel.tex
	latexmk -pdf -output-directory=../compilation logiciel.tex
	mv ../compilation/logiciel.pdf ../imgs

../imgs/slide_intro_process.pdf : slide_intro_process.tex
	latexmk -pdf -output-directory=../compilation slide_intro_process.tex
	mv ../compilation/slide_intro_process.pdf ../imgs

clean :
	@rm -f *.aux *~ *.bbl *.blg *.glg *.glo *.gls *.ist *.log 

.PHONY: $(CIBLE)
