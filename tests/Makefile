TESTS=test1_poisson

$(TESTS).html: $(TESTS).qmd
	quarto render --to html

clean:
	rm $(TESTS).html
