CONTIKI_PROJECT = coap-example-server
all: $(CONTIKI_PROJECT)

# Do not try to build on Sky because of code size limitation
PLATFORMS_EXCLUDE = sky z1

# Include the CoAP implementation
MODULES += os/net/app-layer/coap

# Include CoAP resources
MODULES_REL += ./resources

MODULES += os/services/shell

MAKE_MAC = MAKE_MAC_TSCH

CONTIKI=../../..
include $(CONTIKI)/Makefile.include
