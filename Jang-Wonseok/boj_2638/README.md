## Link
[치즈](https://www.acmicpc.net/problem/2638)

## Topic
- BFS

## Approach

가장자리 (0, 0)으로부터 BFS를 돌아 치즈의 위치와 노출되는 변의 개수를 구한다.

1. BFS를 수행할 큐와 자료형, 방문 체크 배열을 준비한다.
    - `Point`: row, col을 담은 좌표
2. (0, 0)에서부터 BFS를 출발하여 치즈를 만나면 노출 개수를 증가시킨다.
3. 치즈가 더이상 존재하지 않을 때까지 BFS를 반복한다.
    - 치즈의 개수를 따로 저장하고 체크한다.
    - BFS가 끝날 때 걸린 시간을 증가시킨다.
   