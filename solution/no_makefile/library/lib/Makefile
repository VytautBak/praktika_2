CC:=gcc
LIB:=libfilereader.so
SRC:=$(wildcard *.c)
OBJ:=$(SRC:.c=.o)

.PHONY: all clean

all: $(LIB)

$(LIB): $(OBJ)
	$(CC) $(CFLAGS) -fpic -shared -o $@ $^

clean:
	$(RM) $(LIB) $(OBJ)
