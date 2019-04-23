# Para qual plataforma vamos compilar?
TARGET = srf06-cc26xx
BOARD = launchpad/cc1350

CONTIKI = ../../contiki
CONTIKI_WITH_IPV6 = 1
CFLAGS += -g

# Qual nossa aplicação/projeto?
CONTIKI_PROJECT = cliente-udp-sensor
# CONTIKI_PROJECT = servidor-udp cliente-udp-sensor

# Quais outros arquivos precisamos compilar?
PROJECT_SOURCEFILES += uip_utils.c mdns_utils.c

# Há um arquivo com configurações globais do contiki?
CFLAGS += -DPROJECT_CONF_H=\"project-conf.h\"

all: $(CONTIKI_PROJECT)

include ../../Makefile.toolchain
include $(CONTIKI)/Makefile.include
