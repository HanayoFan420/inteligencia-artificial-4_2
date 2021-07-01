import collections
# Algoritmo BFS
def bfs(graph, root):

    visited, queue = set(), collections.deque([root])
    visited.add(root)

    while queue:

        # Quitar un vértice del grafo
        vertice = queue.popleft()
        print(str(vertice) + " ", end="")

        # Ver si hay nodos nuevos por añadir a la cola
        for neighbour in graph[vertice]:
            if neighbour not in visited:
                visited.add(neighbour)
                queue.append(neighbour)

#Ejemplo 1
if __name__ == '__main__':
    graph = {
        0: [1, 2], 
        1: [2], 
        2: [3], 
        3: [1, 2]
        }
print("Camino del algoritmo BFS: ")
bfs(graph, 0)
