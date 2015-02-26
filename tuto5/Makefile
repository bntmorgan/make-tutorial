TARGETS=cible
OBJECTS=main.o 1.o 2.o 3.o
LDFLAGS=
CFLAGS=-Wall -Werror
DEPENDS=$(patsubst %.o, %.dep, $(OBJECTS))

all: $(TARGETS)

cible: $(OBJECTS)
	gcc $(LDFLAGS) -o $@ $^

%.o: %.c %.dep
	gcc $(CFLAGS) -c $<

depend: $(DEPENDS)

%.dep: %.c
	gcc -MM $^ -o $@

include $(wildcard %.dep)

clean:
	rm -fr $(OBJECTS) $(TARGETS) $(DEPENDS)

run:
	./cible
