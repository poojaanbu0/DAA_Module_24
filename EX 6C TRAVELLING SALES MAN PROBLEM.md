# EX 6C TRAVELLING SALES MAN PROBLEM

## AIM:
To Solve Travelling Sales man Problem for the following graph.

![436921662-653921a4-3d7b-4691-9b41-735e80f7af0b](https://github.com/user-attachments/assets/16e336f7-0d06-4d58-a541-ad04b333f8e2)


## Algorithm

1.Take the cost matrix that shows the cost between every pair of cities.

2.Generate all possible orders (permutations) in which the cities can be visited.

3.For each order, calculate the total travel cost, including returning to the starting city.

4.Keep track of the minimum total cost found so far.

5.After checking all possible orders, return the minimum cost as the final answer.

## Program:
```
/*
# Developed by: Pooja A
# Register Number: 212222240072
*/

def tsp_cost(tsp):
    return min(sum(tsp[i][j] for i, j in zip(path, path[1:] + path[:1])) for path in permutations(range(len(tsp))))

from itertools import permutations
tsp = [[-1, 30, 25, 10], [15, -1, 20, 40], [10, 20, -1, 25], [30, 10, 20, -1]]
print("Minimum Cost is :",tsp_cost(tsp))
```

## Output:
![447235374-4ab680e4-b50c-4368-8911-f5cc233598ec](https://github.com/user-attachments/assets/75eac1ba-ccbb-417f-adad-edfabbd434ea)


## Result:
Thus the program was executed successfully for finding the minimum cost to vist all cities.
