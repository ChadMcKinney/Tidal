CONFIG=
HTML_CONFIG=$(CONFIG) --standalone
PDF_CONFIG=$(CONFIG) --latex-engine=xelatex --variable mainfont="Linux Libertine O" --variable sansfont="Linux Biolinum O" --variable geometry="a4paper"

all: tidal.pdf tidal.html

tidal.pdf: tidal.pandoc
	pandoc $(PDF_CONFIG) tidal.pandoc -o tidal.pdf

tidal.html: tidal.pandoc
	pandoc $(HTML_CONFIG) tidal.pandoc -o tidal.html
