CONTIKI_PROJECT = sensortag-coap-server
all: $(CONTIKI_PROJECT)

# Include the CoAP implementation
MODULES += os/net/app-layer/coap

# Include CoAP resources
MODULES_REL += ./resources

MODULES += os/services/shell

MAKE_MAC = MAKE_MAC_TSCH

CONTIKI=../../
include $(CONTIKI)/Makefile.include
