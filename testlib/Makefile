all:
	 gcc -c testlib.c
	 gcc -c main.c
	 gcc -o main testlib.o main.o

test_testlib: clean
	 gcc -c testlib.c
	 gcc -c test_testlib.c
	 gcc -o test_testlib.exe testlib.o test_testlib.o
	 ./test_testlib.exe

test:	 test_testlib

clean:
	 rm *.out *.o *.exe || exit 0

run:
	 gcc -c testlib.c
	 gcc -c main.c
	 gcc -o main.exe testlib.o main.o
	 ./main
