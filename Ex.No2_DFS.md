# Ex.No: 2  Implementation of Depth First Search.

### DATE: 17.02.2024

### REGISTER NUMBER : 212221220063

### AIM: 
To write a python program to implement Depth first Search. 

### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.


### Program:
graph = {
    '1': ['2', '3'],
    '2': ['4', '5'],
    '3': ['6', '7'],
    '4': [],
    '5': [],
    '6': [],
    '7': [],
}

visited = set()

def dfs(node, graph):
    if node not in visited:
        print(node)
        visited.add(node)

        if graph[node]:
            for neighbor in graph[node]:
                dfs(neighbor, graph)
print("DFS order is ")
dfs('1', graph)











### Output:
![image](https://github.com/Yugendaran/AI_Lab_2023-24/assets/128135616/7676a856-b90c-45e0-a46e-94ff210e8ae0)



### Result:
Thus the depth first search order was found sucessfully.
