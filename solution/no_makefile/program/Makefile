CC:=gcc
CPPFLAGS:=-I$(PWD)
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)
BIN:=calculator

PREFIX?=/usr


.PHONY:= all clean install uninstall

all: $(BIN)

$(BIN) : $(OBJ)
	$(CC) $(CPPFLAGS) -o $@ $^

clean:
	rm -f $(BIN) $(OBJ)

install: $(BIN)
	install -d $(PREFIX)/bin
	install -m 777 calculator $(PREFIX)/bin/$(BIN)

uninstall:
	rm -f $(PREFIX)/bin/$(BIN)
 
