# Graph Theory | Institute of Computing - UFAL

## 📌 Description

This project was developed as part of the Graph Theory course in the Computer Science program at the Federal University of Alagoas (UFAL).

The work consists of the implementation of five fundamental graph algorithms, covering classic problems such as:

- Shortest paths
- Minimum spanning trees
- Strongly connected components
- Maximum clique

All algorithms were implemented in C++, with standardized command-line input, modular structure, a `Makefile` for compilation, and support for automated tests via shell script.

---

## 👥 Student:
Leila Maria Biggi de Souza Cavalcante

---

## 🧠 Implemented Algorithms

### 1. Prim's Algorithm
Builds the Minimum Spanning Tree (MST) of a connected and weighted graph by selecting edges of minimum weight without forming cycles.

### 2. Kruskal's Algorithm
Finds the MST by sorting edges by weight and merging components without creating cycles.

### 3. Dijkstra's Algorithm
Determines the shortest path from an initial vertex to all other vertices in a graph with non-negative weights.

### 4. Kosaraju's Algorithm
Identifies all strongly connected components of a directed graph through two DFS passes.

### 5. Carraghan-Pardalos Algorithm
Solves the maximum clique problem by identifying the largest subset of vertices that are all mutually adjacent.

---

## 📁 Repository Structure

```
projeto-grafos/
├── Bat1/                   # Scripts and instances for automated tests
├── Bat2/                   # Automated tests for algorithm 5
├── carraghan_pardalos/     # Algorithm 5: maximum clique
├── dijkstra/               # Shortest path
├── kosaraju/               # Strongly connected components
├── kruskal/                # Minimum spanning tree
├── prim/                   # Minimum spanning tree
```

---

## 🚀 How to Run

### Clone the repository:
```bash
git clone https://github.com/lawtherea/projeto-grafos.git
cd projeto-grafos
```

### Compile an algorithm:
```bash
cd <nome_algoritmo>
make
```

### Run it with the desired parameters, for example:
```bash
./prim -f entrada.txt -i 1 -s
```

### Accepted parameters:
- `-h`: shows help
- `-f <arquivo>`: defines the graph input file
- `-i <vértice>`: defines the initial vertex (when applicable)
- `-s`: prints the solution (edges or path)
- `-o <arquivo>`: redirects output to a file

---

## 🧪 Running the automated tests

```bash
cd Bat1
bash Bat1.sh
```

⚠️ Requirements:
- The `Bat1.sh` script requires `diff` to be installed (available in Git Bash or WSL for Windows users).
- Make sure the binaries (`*.bin`) were generated correctly with the expected names.

---

## 🧪 Script to test the Carraghan-Pardalos algorithm (Bat2.sh)

To run the script, make sure that the executable `carraghan_pardalos.exe` is in the `carraghan_pardalos folder`. Then, run the `Bat2.sh` script from the `Bat2` folder:

```bash
bash Bat2.sh
```

The script will test the Carraghan-Pardalos algorithm on all available test cases and compare the outputs with the corresponding answer files.

## 📝 Notes

- The Carraghan-Pardalos algorithm may return different cliques of the same size, depending on the order in which vertices are visited.
- All files were developed according to the course instructions.

---

> Academic project — Federal University of Alagoas • Institute of Computing • Graph Theory
