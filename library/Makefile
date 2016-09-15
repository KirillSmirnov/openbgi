CROSS =
CC = $(CROSS)gcc
AR = $(CROSS)ar
RANLIB = $(CROSS)ranlib
RM = del /f
CFLAGS = -O2 -Wall
#CFLAGS = /O2 /GL /D "WIN32" /D "NDEBUG" /D "_WINDOWS" /FD /EHsc /MD /W3 /nologo /c /Zi /TP
SRCS = bgi.c server.c client.c ipc.c graphics.c
OBJS = bgi.o server.o client.o ipc.o graphics.o

openbgi.a: $(OBJS)
	$(AR) rvu $@ $(OBJS)
	$(RANLIB) $@

$(OBJS): $(SRCS)
	$(CC) $(CFLAGS) -c $(SRCS)

clean:
	$(RM) *.o
