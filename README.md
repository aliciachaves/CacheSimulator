# Cache Simulator

This Python script simulates a cache memory system with support for various configurations such as cache size, line size, and associativity.

## Description

The script `simulador.py` aims to mimic a cache memory system based on parameters provided through command-line arguments. It reads a memory access file and simulates cache behavior, tracking hits and misses. 

### Features

- **Cache Memory Simulation**: Simulates cache memory operations based on cache size, line size, and associativity configurations.
- **Associativity Support**: Provides support for both fully associative and set-associative caches.
- **Output**: Generates an output file (`output.txt`) with cache contents and hit/miss statistics.

## Usage

The script can be executed from the command line using the following arguments:

```bash
python simulador.py <cache_size> <line_size> <num_sets> <memory_access_file>
```

- `<cache_size>`: Specifies the size of the cache in bytes.
- `<line_size>`: Sets the line size in bytes.
- `<num_sets>`: Defines the associativity or the number of sets for set-associative caches. Use `1` for fully associative caches.
- `<memory_access_file>`: Specifies the file containing memory access information.

## Input File Format

The `memory_access_file` should contain memory addresses in hexadecimal format, with one address per line.

## Output

The script generates an output file (`output.txt`) displaying cache contents and hit/miss statistics. Each line in the output represents a cache line with its index, validity bit, and associated memory address.
