## Link
[트리의 지름](https://www.acmicpc.net/problem/1967)

## Topic
- Recursion

## Approach
 리프 노드까지 가중치를 모두 합한 값중 가장 큰 값을 찾아야 한다. 중간에 끊을 수 없으므로 완전 탐색을 해야하고, 여기에 DFS나 재귀를 이용할 수 있다.

1. 트리의 루트 노드로부터 자식 트리들을 재귀적으로 순회한다.
2. 순회하면서 각 자식 트리의 지름을 구한다.
3. 자식 트리중 긴 두 개의 지름을 택하고 전체 지름을 갱신한다. (더 크다면)
4. 가장 긴 지름에 자신의 가중치를 더해 부모에게 돌려준다.
5. 루트 노드까지 반복한다.
   
## Note
- 자식은 3개 이상일 수 있다.