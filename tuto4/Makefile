TARGETS=cible
OBJECTS=main.o 1.o 2.o 3.o
LDFLAGS=
CFLAGS=-Wall -Werror

all: $(TARGETS)

cible: $(OBJECTS)
	gcc $(LDFLAGS) -o $@ $^

%.o: %.c
	gcc $(CFLAGS) -c $<

depend: $(DEPENDS)

clean:
	rm -fr $(OBJECTS) $(TARGETS)

run:
	./cible
