CC = g++
CFLAGS = -Wall -g
LDFLAGS = -lglfw3 -lGL -lGLEW -lX11 -lXxf86vm -lXrandr -lXi -lpthread

build_check: build_check.o
	$(CC) -o $@ $^ $(LDFLAGS)

build_check.o: build_check.cpp
	$(CC) -c $(CFLAGS) $<

.PHONY: clean test

clean:
	rm *.o
	rm build_check
