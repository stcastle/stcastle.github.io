filename=castle-cv-moderncv

pdf:
	pdflatex ${filename}
	biber ${filename}||true
	pdflatex ${filename}
	pdflatex ${filename}

read:
	evince ${filename}.pdf &

aread:
	acroread ${filename}.pdf

clean:
	rm -f ${filename}.{ps,log,aux,out,dvi,bbl,blg}
