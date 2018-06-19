UNAME := $(shell uname)

ifeq ($(UNAME), Darwin)
    SHLIB_EXT ?= dylib
else ifeq ($(UNAME), Windows)
    SHLIB_EXT ?= dll
else
    SHLIB_EXT ?= so
endif

install:
	$(CC) $(CPPFLAGS) $(CFLAGS) $(LDFLAGS) -O2 -shared -fPIC -I $(prefix)/include extractors.c -o $(prefix)/lib/libtestu01extractors.$(SHLIB_EXT) -L $(prefix)/lib $(RPATH) -lmylib -lprobdist -ltestu01
