#
# Kutkov Oleg (kutkov.o@yandex.ru) (July 2016)
#

CC := gcc
PROGRAM = fancontrol
SRC := main.c dht.c
CFLAGS := -Wall -std=gnu99 -g -ggdb
LDFLAG := -l bcm2835 -lrt
TARGET_DIR := /opt/allsky/bin

all: $(PROGRAM)

$(PROGRAM): $(OBJECTS)
		$(CC) $(CFLAGS) $(SRC) $(LDFLAG) -o $(PROGRAM)

install:
		mkdir -p $(TARGET_DIR)
		cp $(PROGRAM) $(TARGET_DIR)

clean:
		rm -fr $(PROGRAM) $(PROGRAM).o

