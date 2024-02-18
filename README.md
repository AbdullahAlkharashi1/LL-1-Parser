# LL(1) Parsing Algorithm

This repository contains a Python script implementing LL(1) parsing algorithm for context-free grammars (CFGs). LL(1) parsing is a specific type of top-down parsing method commonly used for parsing deterministic context-free languages.

## Overview

LL(1) parsing involves constructing a predictive parsing table based on the given grammar's FIRST and FOLLOW sets. This table guides the parsing process by providing the appropriate production rule to apply at each parsing step.

## Implementation Details

The provided Python script performs the following tasks:

1. **Grammar Representation**: Reads a set of grammar rules from a file named "grammar.txt" and stores them in an ordered dictionary.

2. **FIRST Set Computation**: Calculates the FIRST sets for each non-terminal symbol in the grammar. The FIRST set of a symbol consists of all terminals that begin strings derived from that symbol in one step of derivation.

3. **FOLLOW Set Computation**: Calculates the FOLLOW sets for each non-terminal symbol in the grammar. The FOLLOW set of a non-terminal symbol consists of all terminals that can appear immediately to the right of that symbol in some sentential form.

4. **Parse Table Generation**: Generates a parse table based on the computed FIRST and FOLLOW sets. This parse table determines the next production to apply during parsing based on the current non-terminal and the next input symbol.

5. **Parsing Process**: Parses an input expression using the generated parse table. The parsing process starts from the start symbol and proceeds by making parsing decisions according to the contents of the parse table and the current input symbol.

## Usage

To use the LL(1) parsing script:

1. Ensure you have Python installed on your system.
2. Clone this repository to your local machine.
3. Modify the grammar rules in the "grammar.txt" file to match your specific context-free grammar.
4. Run the Python script and provide an input expression to be parsed.

## Example

An example grammar file ("grammar.txt") and an input expression ("i+i*)$") are provided in the repository for demonstration purposes.

## Contributing

Contributions to this project are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.

