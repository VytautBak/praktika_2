LIB:=libcalculator.so
CC:=gcc
CFLAGS:= 
CPPFLAGS:=
LDFLAGS:= 
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)

PREFIX?=/usr

.PHONY: $(LIB) install uninstall clean

all: $(LIB)

$(LIB): $(OBJ)
	$(CC) $(CPPFLAGS) $(CFLAGS) -shared -fPIC -o $(LIB) $^ $(LDFLAGS)

install: $(LIB)
	install -d $(PREFIX)/include
	install -m 644 math_functions.h $(PREFIX)/include/math_functions.h

uninstall:
	rm -f $(PREFIX)/include/math_functions.h

clean:
	rm -f $(LIB) $(OBJ)
