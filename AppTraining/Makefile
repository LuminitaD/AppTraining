CFLAGS_DBUS = $(shell pkg-config --cflags --libs dbus-1 glib-2.0 gio-unix-2.0 gobject-2.0 gthread-2.0)
CFLAGS_DBUS_GLIB = $(shell pkg-config --cflags --libs dbus-glib-1)
CFLAGS_GIO  = $(shell pkg-config --cflags --libs gio-2.0)

CFLAGS = -g -Wall -Werror

all:
	gcc -o build/myApp src/*.c $(CFLAGS) $(CFLAGS_DBUS) $(CFLAGS_DBUS_GLIB) $(CFLAGS_GIO) -I include


clean:
	rm -f build/*
