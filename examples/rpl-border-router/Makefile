CONTIKI_PROJECT = border-router
all: $(CONTIKI_PROJECT)
CONTIKI = ../..

# The BR is either native or embedded, and in the latter case must support SLIP
PLATFORMS_EXCLUDE = nrf52dk z1

MAKE_MAC = MAKE_MAC_TSCH

# Include RPL BR module
MODULES += os/services/rpl-border-router
# Include webserver module
MODULES_REL += webserver
# Include optional target-specific module
include $(CONTIKI)/Makefile.identify-target
MAKE_MAC = MAKE_MAC_TSCH
MODULES += os/services/shell
MODULES_REL += $(TARGET)

TARGET = cc26x0-cc13x0
BOARD = launchpad/cc1350
PORT = /dev/ttyACM0

include $(CONTIKI)/Makefile.include
