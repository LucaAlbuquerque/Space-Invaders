CC = gcc
CFLAGS = -Wall -Wextra -pthread -g
LDFLAGS = -lm -lncurses

SRCFILES = $(wildcard *.c)
OBJFILES = $(SRCFILES:.c=.o)
EXECUTABLE = start

all: $(EXECUTABLE)

$(EXECUTABLE): $(OBJFILES)
	$(CC) $(CFLAGS) -o $@ $^ $(LDFLAGS)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f *.o $(EXECUTABLE)
