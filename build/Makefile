SLIDES := $(patsubst %.md,%.slides.pdf,$(wildcard *.md slides/*.md))
DIAGRAMS := $(patsubst %.dot,%-dot.pdf,$(wildcard diagrams/*.dot))
TEMPLATE := ./beamer.template

HIGHLIGHT_STYLE=pygments
# Highlight styles: pygments kate monochrome espresso haddock tango zenburn

PANDOC_OPTS := -t beamer --template=$(TEMPLATE)\
	--slide-level 2 \
	--highlight-style=$(HIGHLIGHT_STYLE) \
	--pdf-engine xelatex

all : $(SLIDES) $(HANDOUTS)

%.slides.pdf : %.md $(DIAGRAMS) $(TEMPLATE)
	pandoc $< $(PANDOC_OPTS) -o $@

%-dot.pdf: %.dot
	dot -Tps2 $< -o $@.ps
	ps2pdf $@.ps $@
	rm $@.ps
clean:
	rm -f $(SLIDES) $(DIAGRAMS)

diagrams: $(DIAGRAMS)
