# Speller

A fast spell-checker implementation in C using hash tables for dictionary lookups, created as part of Harvard's CS50 course.

## Overview

This program efficiently checks for misspelled words in a text by comparing them against a dictionary. It uses a hash table data structure for O(1) average-case lookup time and provides detailed performance metrics.

## Features

- Custom hash function for optimal distribution
- Case-insensitive word comparison
- Memory-efficient implementation
- Performance benchmarking for:
  - Dictionary loading time
  - Word checking time
  - Memory unloading time
  - Total runtime analysis

## Usage

### Prerequisites
- GCC or Clang compiler
- Make build system

### Compilation
```bash
make speller
```

### Running the Program
```bash
./speller [dictionary] text
```
Arguments:
- `[dictionary]`: Optional path to dictionary file (default: `dictionaries/large`)
- `text`: Text file to spell-check

### Example
```bash
./speller texts/cat.txt
```

## Implementation Details

The program is built around five main functions:

1. `load`: Loads dictionary into memory
2. `hash`: Converts strings to hash table indices
3. `check`: Looks up words in the hash table
4. `size`: Returns dictionary word count
5. `unload`: Frees allocated memory

## Output

The program outputs:
- List of misspelled words
- Statistics including:
  - Number of misspelled words
  - Total words in dictionary
  - Total words in text
  - Timing data for each operation

## Contributing

This is a learning project completed as part of CS50. While it's not open for contributions, feel free to fork and experiment with your own improvements!

## License

This project is part of Harvard's CS50 coursework. Please check [CS50's Academic Honesty rules](https://cs50.harvard.edu/x/2024/honesty/) before using this code.
