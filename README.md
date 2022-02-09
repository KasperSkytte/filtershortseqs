# Filter short sequences
filterShortSeqs is a small program written in C++ which filters DNA sequences from an input FASTA file if there are any other 100% identical, but longer sequences present in the FASTA file. The sequences are dereplicated initially. Multithreaded using OpenMP.

## Requirements
 - `cmake`
 - `make`
 - A C++ compiler
 - probably others...

## Compilation
Run `cmake CMakeLists.txt` and then `make`. Compiles into a single binary `filterShortSeqs` in the current folder.

## Usage
```
$ ./filterShortSeqs 
missing input file
missing output file
usage: filterShortSeqs <input_file> <output_file> <threads>
```
