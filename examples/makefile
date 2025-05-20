CC=gcc
CFLAGS=-I../include
LDFLAGS=-L../lib
LOADLIBES=-lregis -lm

all: regis_demo planet_motion 3d_arduino

planet_motion: planet_motion.o planet_motion_fns.o 

CFLAGS+=-I.
3d_arduino:

clean:
	$(RM) regis_demo planet_motion 3d_arduino *.o
