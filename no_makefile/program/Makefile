CC:=gcc
CPPFLAGS:=-I$(PWD)
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)
BIN:=calculator

.PHONY:= $(BIN) clean

all: $(BIN)

$(BIN) : $(OBJ)
	$(CC) $(CPPFLAGS) -o $@ $^

clean:
	rm -f $(BIN) $(OBJ)
