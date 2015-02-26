TARGETS=cible
OBJECTS=main.o 1.o 2.o 3.o
LDFLAGS=
CFLAGS=-Wall -Werror

all: $(TARGETS)

cible: $(OBJECTS)
	gcc $(LDFLAGS) -o $@ $^

1.o: 1.c
	gcc $(CFLAGS) -c $^

2.o: 2.c
	gcc $(CFLAGS) -c $^

3.o: 3.c
	gcc $(CFLAGS) -c $^

main.o: main.c
	gcc $(CFLAGS) -c $^

clean:
	rm $(OBJECTS) $(TARGETS)

run:
	./cible
