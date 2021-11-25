CFLAGS=-W -Wall -I. -g

SRC=sim.c cpu.c timing.c vcd.c
DEPS=`sdl2-config --libs --cflags` -lSDL2_image $(LDFLAGS)

all: vt52

vt52: $(SRC) defs.h ../common/xsdl.h ../common/opengl.h
	$(CC) -o $@ $(SRC) $(DEPS)

clean:
	rm -f vt52 *.o
