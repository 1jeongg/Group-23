## Link
[도시 분할 계획](https://www.acmicpc.net/problem/1647)

## Topic
- MST (Kruskal / Prim)

## Approach

최소 스패닝 트리를 구하면 모든 마을을 연결하는 최소 비용의 도로 집합을 구할 수 있고, 이중 가장 유지비가 큰 도로를 끊으면 두 도시로 분할된다.

1. 최소 스패닝 트리를 진행할 우선순위 큐를 준비한다.
    - 우선순위 큐에 간선을 모두 넣는다. (오름차순)
2. 간선을 하나씩 꺼내면서 사이클을 검사하고, 없으면 두 정점을 병합한다.
    - 사이클 검사와 병합은 Union Find를 이용한다.
3. 우선순위 큐가 모두 비었거나, 간선 개수가 정점보다 1개 작을 때 종료한다.
    - MST 이후 간선 개수가 부족하면 실패이다.