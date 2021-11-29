CC:=gcc
BIN:=filereaderexample
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)
LDFLAGS:=-L../lib -lfilereader
CPPFLAGS:=-I../lib

PREFIX?=/usr

.PHONY: all clean install uninstall

all: $(BIN)

$(BIN): $(OBJ)
	$(CC) $(CPPFLAGS) $(CFLAGS) -o $@ $^ $(LDFLAGS)

clean:
	$(RM) $(BIN) $(OBJ)

install: $(BIN)
	install -d $(PREFIX)/bin
	install -m 777 $(BIN) $(PREFIX)/bin/$(BIN)

uninstall:
	rm -f $(PREFIX)/bin/$(BIN)
