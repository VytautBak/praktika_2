
.PHONY: lib src clean install uninstall

all: lib src

lib:
	$(MAKE) -C $@

src: lib
	$(MAKE) -C $@

clean:
	$(MAKE) -C src clean
	$(MAKE) -C lib clean

install: src lib
	$(MAKE) -C src install
	$(MAKE) -C lib install

uninstall: 
	$(MAKE) -C src uninstall
	$(MAKE) -C lib uninstall
