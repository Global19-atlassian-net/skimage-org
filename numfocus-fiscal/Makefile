DOC=numfocus-fiscal-sponsorship.md
PDF=$(DOC:%.md=%.pdf)

.PHONY: doc
doc:
	pandoc $(DOC) \
		-f gfm \
		--pdf-engine=xelatex \
		-V "mainfont=Noto Sans" \
		-V colorlinks=true \
		-V linestretch=1.25 \
		-o $(PDF)

.PHONY: clean
clean:
	rm $(PDF)
