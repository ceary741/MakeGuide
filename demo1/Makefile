CC = clang
CFLAGS = -O3 -DHELLO_MSG='"Hello Var\n"'

main : main.c main.h
	echo $^
	$(CC) $(CFLAGS) -o $@ $<
clean : 
	rm -rf main
