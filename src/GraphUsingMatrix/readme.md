<!--
|----------------------------------------------------------------------------------------------------|
| Memory Address | Object Type                       | Content                                       |
|----------------|-----------------------------------|-----------------------------------------------|
| 0x001          | ArrayList<GraphNode>             | size: 5                                        | // Size of the list
|                |                                   | elements: [0x002, 0x003, 0x004, 0x005, 0x006] | // References to GraphNode objects
|----------------|-----------------------------------|-----------------------------------------------|
| 0x002          | GraphNode                         | name: "A"                                     | // NodeA instance
|                |                                   | index: 1                                      | // ID of NodeA
|----------------|-----------------------------------|-----------------------------------------------|
| 0x003          | GraphNode                         | name: "B"                                     | // NodeB instance
|                |                                   | index: 2                                      | // ID of NodeB
|----------------|-----------------------------------|-----------------------------------------------|
| 0x004          | GraphNode                         | name: "C"                                     | // NodeC instance
|                |                                   | index: 3                                      | // ID of NodeC
|----------------|-----------------------------------|-----------------------------------------------|
| 0x005          | GraphNode                         | name: "D"                                     | // NodeD instance
|                |                                   | index: 4                                      | // ID of NodeD
|----------------|-----------------------------------|-----------------------------------------------|
| 0x006          | GraphNode                         | name: "E"                                     | // NodeE instance
|                |                                   | index: 5                                      | // ID of NodeE
|----------------|-----------------------------------|-----------------------------------------------|
| 0x007          | Graph                             | nodeList: 0x001                               | // Graph instance holding nodeList
|----------------|-----------------------------------|-----------------------------------------------|
| 0x008          | int[][] (adjacency matrix)        | [0, 1, 1, 1, 0]                               | // Row for A (edges to B, C, D)
|                |                                   | [1, 0, 0, 0, 1]                               | // Row for B (edges to A, E)
|                |                                   | [1, 0, 0, 1, 0]                               | // Row for C (edges to A, D)
|                |                                   | [1, 0, 1, 0, 1]                               | // Row for D (edges to A, C, E)
|                |                                   | [0, 1, 0, 1, 0]                               | // Row for E (edges to B, D)
|----------------------------------------------------------------------------------------------------|
--> 
