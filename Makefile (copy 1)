# Project: SDLPoP
# Makefile created by Dev-C++ 4.9.9.2

CC   = /run/media/raboten/c03df044-bb85-4f9c-a53f-e537b8a024a0/mipsel-linux-uclibc/usr/bin/mipsel-linux-gcc
OBJ  = main.o data.o seg000.o seg001.o seg002.o seg003.o seg004.o seg005.o seg006.o seg007.o seg008.o seg009.o
LIBS =  `sdl-config --libs` -l"SDL_image" -l"SDL_mixer"
INCS =  
BIN  = prince
CFLAGS = $(INCS) -Wall -pedantic -std=gnu99
RM = rm -f
HFILES   = common.h config.h data.h proto.h types.h

.PHONY: all all-before all-after clean clean-custom

all: all-before $(BIN) all-after


clean: clean-custom
	${RM} $(OBJ) $(BIN)

$(BIN): $(OBJ)
	$(CC) $(OBJ) -o $(BIN) $(LIBS)

%.o: %.c $(HFILES)
	$(CC) -c $< $(CFLAGS)
