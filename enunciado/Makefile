# Variables
CC = gcc
CFLAGS = -Wall -Wextra
OBJS = build.o command.o execution.o io_prompt.o main.o parser.o shell.o stack.o

# Target principal
all: wish

# Compilación del programa
wish: $(OBJS)
	$(CC) $(CFLAGS) -o wish $(OBJS)

# Reglas de compilación para cada archivo objeto
build.o: ./build.c
	$(CC) $(CFLAGS) -c ./build.c

command.o: ./command.c
	$(CC) $(CFLAGS) -c ./command.c

execution.o: ./execution.c
	$(CC) $(CFLAGS) -c ./execution.c

io_prompt.o: ./io_prompt.c
	$(CC) $(CFLAGS) -c ./io_prompt.c

main.o: ./main.c
	$(CC) $(CFLAGS) -c ./main.c

parser.o: ./parser.c
	$(CC) $(CFLAGS) -c ./parser.c

shell.o: ./shell.c
	$(CC) $(CFLAGS) -c ./shell.c

stack.o: ./stack.c
	$(CC) $(CFLAGS) -c ./stack.c

# Limpieza
clean:
	rm -f *.o wish
