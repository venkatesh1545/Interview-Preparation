### 1st Question


### 2nd Question

```python
print("Enter bucket size, outgoing rate, number of inputs and incoming size ")
bucketsize = int(input())
outgoing = int(input())
n = int(input())
incoming = int(input())
store = 0
while n != 0:
    print("Incoming size is ", incoming)
    if incoming <= (bucketsize-store):
        store += incoming
        print("Bucket buffer size is ", store, "out of ", bucketsize)
    else:
        print("Packet loss: ", (incoming - (bucketsize-store)))
        store= bucketsize
        print("Bucket buffer size is ", store, " out of ", bucketsize)
    store -= outgoing
    if store < 0:
        store = 0
    print("After outgoing: ", store, " packets left out of ", bucketsize, "in buffer")
    n = n-1

```

### Output:
```
Enter bucket size, outgoing rate, number of inputs and incoming size
300
50
2
200
Incoming size is  200
Bucket buffer size is  200 out of  300
After outgoing:  150  packets left out of  300 in buffer
Incoming size is  200
Packet loss:  50
Bucket buffer size is  300  out of  300
After outgoing:  250  packets left out of  300 in buffer
```


### 3rd question
```python
INF = 1000

# Function to find the vertex with the minimum distance
def search_min(length, se, n):
    mi = INF
    v = -1
    for i in range(n):
        if not se[i] and length[i] < mi:
            mi = length[i]
            v = i
    return v

# Input adjacency matrix and initialize variables
n = int(input("Enter no of vertices: "))
print("Enter the adjacency matrix: ")
graph = []
for i in range(n):
    graph.append(list(map(int, input().split())))

s = int(input("Enter source node: "))

# Initialization
se = [0] * n  # Visited set
length = [INF] * n  # Distance from source
path = [-1] * n  # Predecessor for each vertex

length[s] = 0  # Distance to source is 0
path[s] = -1  # Source has no predecessor

# Dijkstra's Algorithm
for _ in range(n - 1):
    u = search_min(length, se, n)
    if u == -1:  # If no vertex can be selected, stop
        break
    se[u] = 1
    for v in range(n):
        if not se[v] and graph[u][v] != 0 and length[u] + graph[u][v] < length[v]:
            length[v] = length[u] + graph[u][v]
            path[v] = u

# Function to reconstruct the path
def reconstruct_path(end, start):
    shortest_path = []
    while end != -1:
        shortest_path.append(end)
        end = path[end]
    #shortest_path.reverse()
    return shortest_path

# Output the shortest paths
print(f"From (source vertex) to {s}")
print("\tPath\t\tLength\t\tShortest Path")

for i in range(n):
    if i != s:
        print(f"\t{i}\t\t{length[i]}\t\t", end="")
        shortest_path = reconstruct_path(i, s)
        print(" -> ".join(map(str, shortest_path)))
```

### Output:
```
Enter no of vertices: 4
Enter the adjacency matrix: 
0 6 0 1
6 0 2 4
0 2 0 1
1 4 1 0
Enter source node: 0
From (source vertex) to 0
        Path            Length          Shortest Path
        1               4               1 -> 2 -> 3 -> 0
        2               2               2 -> 3 -> 0
        3               1               3 -> 0

```
