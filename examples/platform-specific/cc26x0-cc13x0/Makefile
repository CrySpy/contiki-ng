CONTIKI_PROJECT = cc26x0-demo

PLATFORMS_ONLY = cc26x0-cc13x0

all: $(CONTIKI_PROJECT)

MAKE_MAC = MAKE_MAC_TSCH

PORT = /dev/ttyACM0

MODULES += os/services/shell

CONTIKI = ../../..
include $(CONTIKI)/Makefile.include
