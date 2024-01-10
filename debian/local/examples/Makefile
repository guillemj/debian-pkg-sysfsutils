#
# Makefile for sysfsutils examples.
#

VPATH = .:/usr/share/doc/libsysfs-dev/examples

PROGS = \
	dlist_test \
	get_device \
	get_driver \
	get_module \
	# EOL

PKG_CONFIG ?= pkg-config

CFLAGS += $(shell $(PKG_CONFIG) --cflags libsysfs) -I/usr/include/sysfs/
LDLIBS += $(shell $(PKG_CONFIG) --libs libsysfs)

all: $(PROGS)
