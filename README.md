# homework-04-dijkstra

graphs_csirhall

A Python package for graph algorithms, including Dijkstra's shortest path.
The project is structured for easy installation, testing, and future extension with more graph algorithms.

Installation

Clone the repository and install locally with:

git clone https://github.com/csirhall/dijkstra-sp.git
cd dijkstra-sp
pip install .

Usage

Run the shortest path algorithm using the provided test.py script:

python src/test.py graph.txt


This will:

Read the graph from graph.txt.

Compute the shortest distances from source node 0.

Print the distances and the shortest paths.

Graph File Format

The graph file should:

Start with the number of vertices.

List edges in the format:

source destination weight

Example
9
0 1 4
0 7 8
1 2 8
1 7 11
2 3 7
2 8 2
2 5 4
3 4 9
3 5 14
4 5 10
5 6 2
6 7 1
6 8 6
7 8 7

Example Output

For the graph above, the program prints:

Shortest distances from 0:
[0, 4, 12, 19, 28, 16, 18, 8, 14]
spf to 0: []
spf to 1: [0]
spf to 2: [0, 1]
spf to 3: [0, 1, 2]
spf to 4: [0, 1, 2, 3]
spf to 5: [0, 1, 2]
spf to 6: [0, 7]
spf to 7: [0]
spf to 8: [0, 1, 2]