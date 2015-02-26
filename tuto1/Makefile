# Règle par défaut : déclarée en premier
all: cible1

cible1: dependance1 dependance2
	cat dependance1 dependance2 > cible1

dependance1:
	echo "contenu 1" > dependance1

clean:
	rm dependance1 cible1
