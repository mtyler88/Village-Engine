CC=g++
CFLAGS=-c -Wall
LDFLAGS= 
SDLFLAGS=-lSDL2 -lSDL2_gfx
SOURCES=main.cpp Vec.cpp Mat.cpp Transform.cpp LTimer.cpp EventManager.cpp Event.cpp GameManager.cpp Entity.cpp EntityManager.cpp Console.cpp
OBJECTS=$(SOURCES:.cpp=.o)
EXECUTABLE=VillageEngine

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) $(SDLFLAGS) -o $@

.cpp.o:
	$(CC) $(CFLAGS) $< -o $@


.PHONY: clean
clean:
	rm $(EXECUTABLE) $(OBJECTS)
