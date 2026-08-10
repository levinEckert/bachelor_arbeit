##
## macrodefinitions 
##
LATEX        = pdflatex
BIBER        = biber
SRC          = main
LATEX_FLAGS  = -interaction=nonstopmode -halt-on-error -file-line-error
REMOVE       = *.tex~ *.aux *.glo *.gls *.cb *.dvi *.log *.toc *.lof *.bbl *.blg *.ilg *.cb? *.idx *.out

##
## rules
##
.PHONY: all quick clean

all : 
	$(LATEX) $(LATEX_FLAGS) $(SRC)
	$(BIBER)  $(SRC)
	$(LATEX) $(LATEX_FLAGS) $(SRC)
	$(LATEX) $(LATEX_FLAGS) $(SRC)

quick :
	$(LATEX) $(LATEX_FLAGS) $(SRC)

clean :
	rm -fv $(REMOVE)
