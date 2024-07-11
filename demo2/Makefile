lec.pdf : save-temps
	make clean-temps

save-temps : pic.svg lec.tex
	pdflatex -shell-escape lec.tex

pic.svg : data plot.plt
	gnuplot plot.plt

data : data_gen.sh
	bash data_gen.sh

clean-temps : 
	rm -rf svg-* lec.aux lec.log pic.svg data

clean : 
	rm -rf svg-* lec.aux lec.log lec.pdf pic.svg data
