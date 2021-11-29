CC:=gcc
CPPFLAGS:=-I$(PWD)
SRC:=$(wildcard *.c)
OBJS:=$(SRC:.c=.o)
BIN:=calculator

.PHONY: all clean

all: $(BIN)

$(BIN): $(OBJS)
	$(CC) $(CPPFLAGS) -o $@ $^ 

clean:
	rm -f $(BIN) $(OBJS)
