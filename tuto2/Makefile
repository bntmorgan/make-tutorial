# Variables
TARGETS=cible1
OBJECTS=dependance1

# Règle par défaut : déclarée en premier
all: $(TARGETS)

cible1: $(OBJECTS)
	cat $^ > $@

dependance1:
	echo "contenu 1" > $@

clean:
	rm $(OBJECTS) $(TARGETS)
