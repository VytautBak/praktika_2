compiler:=gcc
Flags:=-Wall -Ipwd
OBJS:=main.o math_functions.o
BIN:=calculator

all: $(BIN)

$(BIN): main.o math_functions.o
	$(compiler) $(Flags) -o $(BIN) main.o 

clean:
	rm -f $(BIN) $(OBJS)
