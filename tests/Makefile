TESTS=test0_custom_FE test1_poissonP1xP1
TESTS_HTML=$(TESTS).html
TESTS_PDF=$(TESTS).pdf

all: $(TESTS_HTML) $(TESTS_PDF)

$(TESTS_HTML): $(TESTS).qmd
	quarto render $< --to html 

$(TESTS_PDF): $(TESTS).qmd
	quarto render $< --to pdf 

clean:
	rm $(TESTS_HTML) $(TESTS_PDF) 
	rm -rf $(TESTS)_files
