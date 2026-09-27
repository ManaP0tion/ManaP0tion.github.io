---
title: BFS 알고리즘
date: 2026-09-24 12:00:00 +0900
cstegories: [Algorithm]
tags: [알고리즘, BFS, 파이썬]
---

```python
from collections import deque

def bfs(graph, start, visited):
    queue = deque([start])
    visited[start] = True
    
    while queue:
        v = queue.popleft()
        print(v, end=" ")
        
        for i in graph[v]:
            if not visited[i]:
                queue.append(i)
                visited[i] = True

```


