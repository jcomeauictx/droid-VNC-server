all: libsuinput.so
suinput.o: suinput.c
	gcc -fPIC -o $@ -c $<
libsuinput.so: suinput.o
	gcc -shared -o $@ $<
clean:
	rm -f *.o
distclean: clean
	rm -f *.so
