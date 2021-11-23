
.PHONY: lib src clean

all: lib src

lib:
	$(MAKE) -C $@

src: lib
	$(MAKE) -C $@

clean:
	$(MAKE) -C src clean
	$(MAKE) -C lib clean


