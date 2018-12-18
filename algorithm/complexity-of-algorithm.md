# Complexity of algorithm

계산복잡도란?(Complexity) - 어떤 알고리즘이 문제를 풀기위해 해야하는 계산이 얼마나 복잡한지 나타낸 정도

대문자 O 표기법을 가장 많이 사용한다('빅 오' 표기법이라고도 부른다)

1부터 n까지의 합을 구하는 알고리즘으로 비교
```python
def sum(n):
    sum = 0
    for i in range(1, n+1):
        sum += i

    return sum
```
첫 번째 알고리즘은 입력크기 n에 대해 사칙연산(덧셈)을 n번 해야한다.

즉, 필요한 계산 횟수가 입력크기에 '정비례'하므로 계산복잡도는 O(n)이 된다.
```python
def sum(n):
    sum = n * (n + 1) // 2
    return sum
```
두 번째 알고리즘은 입력크기 n과 무관하게 사칙연산을 3번만 하면된다.

즉, 필요한 계산횟수가 입력크기와 무관하므로 계산복잡도는 O(1)이 된다.

## 계산복잡도 : 시간복잡도와 공간복잡도

시간복잡도는 어떤 알고리즘을 수행하는 데 얼마나 오랜 시간이 걸리는가?이며 공간복잡도는 얼마나 많은 공간(메모리/기억장소)이 필요한지 분석한 것이다. 위에서 분석한 것은 시간 복잡도에 따른 기준이다.