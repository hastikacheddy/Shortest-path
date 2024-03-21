## How it works

1. It will prompt the user to enter a number of nodes.
2. Then the program will generate random x, y coordinates of the number of nofes entered by the user.
3. These nodes are then used to create a complete graph which is stored as an adjacency matrix.
4. The shortest path between every two consecutive nodes is then calculated using the floyd warshall algorithm.
5. Then, all the possible permutations of nodes are generated, which will be used to find the shortest path, each of these permutations will represent the order of visiting the nodes in the graph.
6. A path's cost will be equal to the sum of all shortest paths between every two consecutive nodes.
7. The cost of the current permutation calculated is checked whether it is less than any previous cost calculated. The permutation with the minimum cost will be the shortest path.
8. The GUI will then draw and display that path and outputs its length and path.

## Screenshots of the application in operation

1. Output when 4 nodes is entered.

   ![image](https://github.com/hastikacheddy/Shortest-path/assets/59787014/39d1293f-3e36-465f-af9d-beb4e8028670)

2. Output when 9 nodes is entered.

   ![image](https://github.com/hastikacheddy/Shortest-path/assets/59787014/584b23f2-36fd-45e8-9f86-778d252fb8bc)

