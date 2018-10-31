# module_lldp_get Makefile

TARGET_SO = lldp_get.so

top_srcdir	= /usr/local/src/zabbix/

CC	= gcc
CFLAGS	= -g -O2 -Wall -fPIC $(TARGET_FLAGS)
LDFLAGS	=
LDFLAGS_SO	= -shared
INCLUDES = -I$(top_srcdir)/include
LIBS	=

OBJS	= \
	lldp_get.o

all:	$(TARGET_SO)

$(TARGET_SO):	$(OBJS)
	$(CC) $(LDFLAGS_SO) -o $@ $(OBJS) $(LIBS)

clean:
	rm -f $(TARGET_SO) $(OBJS)

.c.o:
	$(CC) $(CFLAGS) $(INCLUDES) -c $<
