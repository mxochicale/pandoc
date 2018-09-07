SLIDES := $(patsubst %.md,%.md.slides.pdf,$(wildcard *.md))

all : $(SLIDES) $(HANDOUTS)

%.md.slides.pdf : %.md
	pandoc $^ -t beamer --slide-level 2 -o $@

clean : 
	rm -f $(SLIDES)
