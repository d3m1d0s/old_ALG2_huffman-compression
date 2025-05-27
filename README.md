# Huffman Compression Algorithm

This project implements a classic **Huffman Coding** compression algorithm in C++.  
It was developed as part of the *Algorithms II* course at **VSB – Technical University of Ostrava**.

The application performs lossless text compression by building a binary Huffman tree based on character frequencies, storing compressed data in a binary format, and then decompressing it back.

---

## Features

- Lossless text compression with Huffman coding
- Frequency analysis of input characters
- Huffman tree construction and traversal
- Bit-level file compression and decompression
- Binary output format
- CLI interface
- CMake support
- Doxygen documentation ready

---

## Project Structure

```

huffman-compression
├── main.cpp                 # Main implementation file
├── input.txt                # Example text input
├── output.txt               # Decompressed output
├── compressed.bin           # Compressed file
├── compressed.bin.huff      # Huffman-coded binary file
├── CMakeLists.txt           # CMake build script
├── Doxyfile                 # Doxygen config

````

---

## Build Instructions

Make sure you have CMake and a C++ compiler installed:

```bash
git clone https://github.com/your-username/huffman-compression.git
cd huffman-compression
mkdir build && cd build
cmake ..
make
````

---

## Usage Example

To compress a file:

```bash
./huffman-compression input.txt compressed.bin
```

To decompress:

```bash
./huffman-compression compressed.bin output.txt
```

---

## Algorithm Overview

Huffman coding is a **greedy algorithm** used for data compression. It assigns shorter binary codes to more frequent characters and longer codes to less frequent ones, reducing the overall data size without loss.

Steps:

1. Analyze character frequency in the input.
2. Build a binary tree with minimum-weight nodes merged iteratively.
3. Generate binary codes by traversing the tree.
4. Encode the file using generated codes and store compressed output.

---

## Academic Context

This project was developed for the **Algorithms II** course (*ALG2*)
Faculty of Electrical Engineering and Computer Science
**VSB – Technical University of Ostrava**

It demonstrates practical skills in:

* Tree and priority queue data structures
* Bitwise operations
* File I/O in C++
* Efficient algorithmic design

---

## License

This project is for educational purposes only.

---

> “Programs must be written for people to read, and only incidentally for machines to execute.”
>  Harold Abelson    
