LIB:=libcalculator.so
CC:=gcc
CFLAGS:= 
CPPFLAGS:=
LDFLAGS:= 
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)

PREFIX?=/usr

.PHONY: all install uninstall clean

all: $(LIB)

$(LIB): $(OBJ)
	$(CC) $(CPPFLAGS) $(CFLAGS) -shared -fPIC -o $(LIB) $^ $(LDFLAGS)

install: $(LIB)
	install -d $(PREFIX)/include
	install -m 644 math_functions.h $(PREFIX)/include/math_functions.h
	install -d $(PREFIX)/lib
	install -m 644 libcalculator.so $(PREFIX)/lib/$(LIB)

uninstall:
	rm -f $(PREFIX)/include/math_functions.h
	rm -f $(PREFIX)/lib/$(LIB)
clean:
	rm -f $(LIB) $(OBJ)
