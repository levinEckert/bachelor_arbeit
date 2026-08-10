##
## macrodefinitions 
##
LATEX        = pdflatex
BIBER        = biber
SRC          = main
REMOVE       = *.tex~ *.aux *.glo *.gls *.cb *.dvi *.log *.toc *.lof *.bbl *.blg *.ilg *.cb? *.idx *.out

##
## rules
##
all : 
	$(LATEX)  $(SRC)
	$(BIBER)  $(SRC)
	$(LATEX)  $(SRC) 
	$(LATEX)  $(SRC)

clean :
	rm -fv $(REMOVE)
