CC:=gcc
LIB:=libfilereader.so
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)

PREFIX?=/usr

.PHONY: all clean install uninstall

all: $(LIB)

$(LIB): $(OBJ)
	$(CC) $(CFLAGS) -fpic -shared -o $@ $^

clean:
	$(RM) $(LIB) $(OBJ)

install: $(LIB)
	install -d $(PREFIX)/lib
	install -d $(PREFIX)/include
	install -m 644 $(LIB) $(PREFIX)/lib/$(LIB) 
	install -m 644 file_reader.h $(PREFIX)/include/file_reader.h 

uninstall: 
	rm -f $(PREFIX)/lib/$(LIB)
	rm -f $(PREFIX)/include/file_reader.h
