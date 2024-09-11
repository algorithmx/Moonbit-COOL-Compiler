ANTLR_JAR = /home/dabajabaza/Documents/Research/Moonbit-COOL-Compiler/bin/antlr-4.13.2-complete.jar
ANTLR = java -jar $(ANTLR_JAR)
ANTLR_OUT_DIR = ../java
PACKAGE = minimoonbit2024
ANTLR_FLAGS = -no-listener -visitor -package $(PACKAGE)
LEXER = MiniMoonBitLexer
PARSER = MiniMoonBit

%: all

all:
	$(ANTLR) $(ANTLR_FLAGS) -o $(ANTLR_OUT_DIR)/$(PACKAGE)/ -lib $(ANTLR_OUT_DIR)/$(PACKAGE)/ $(PARSER).g4
	echo "\033[0;32m[SUCCESS]\033[0m Generated $(PARSER).java"

clean:
	rm -rf ../java/$(PACKAGE)/*.class
	rm -rf ../java/$(PACKAGE)/$(PARSER)*.java
	rm -rf ../java/$(PACKAGE)/$(PARSER)*.tokens
	echo "\033[0;34m[INFO]\033[0m Clean up ../java/$(PACKAGE)"
