ANTLR_JAR = /home/dabajabaza/Documents/Research/Moonbit-COOL-Compiler/bin/antlr-4.13.2-complete.jar
PACKAGE = minimoonbit2024

%: all

all:
	javac -cp $(ANTLR_JAR) -Xlint ${PACKAGE}/*.java
	echo "\033[0;32m[SUCCESS]\033[0m Generated $(PACKAGE).java"

clean:
	rm -f ${PACKAGE}/*
	echo "\033[0;34m[INFO]\033[0m Clean up ${PACKAGE}/*"
