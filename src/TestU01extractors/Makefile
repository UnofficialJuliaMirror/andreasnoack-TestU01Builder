
install:
	$(CC) $(CPPFLAGS) $(CFLAGS) $(LDFLAGS) -O2 -shared -fPIC -I $(prefix)/include extractors.c -o $(prefix)/lib/libtestu01extractors.$(SHLIB_EXT) -L $(prefix)/lib $(RPATH) -lmylib -lprobdist -ltestu01

# Makefile debugging trick:
# call print-VARIABLE to see the runtime value of any variable
print-%:
	@echo '$*=$($*)'
