# Filter short sequences
filterShortSeqs is a small program written in C++ which filters DNA sequences from an input FASTA file if there are any other 100% identical, but longer sequences present in the FASTA file. The sequences are dereplicated initially, and the relative order of the sequences in the input file are preserved in the output file. Multithreaded using OpenMP. 

Credit to [Nick Green](https://github.com/nickgreensgithub) for creating it for use in [AutoTax](https://github.com/kasperskytte/autotax).

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
