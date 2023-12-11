---
title: BruteForce 완전 탐색
author: RyuRain
date: 2023-12-02 12:40:00 +0900
categories: [Algorithm, BruteForce]
tags: [algorithm,bruteforce]
math: true
mermaid: true
image:
  path: /assets/img/posts/algorithm.png
---

## Brute Force 완전 탐색

Brute Force를 단순회 사전적 의미로 해석하면 (정제되지 않은) "난폭한 힘, 폭력"이란 뜻을 가진 
조합 가능한 모든 경수의 수를 하나씩 대입해 보는 방식이다.

## Brute Force 장단점

### 장점
1. 정확도 100%를 보장한다.
2. 빠르게 구현이 가능하다.
3. 거의 완벽하게 병렬 작업이 가능하다.

### 단점
복잡도(Complexity)에 매우 민감하다.<br>
즉 복잡도에 따라 실행 시간이 매우 커진다. 위 장점을 모두 상쇄시키는 단점이다.
## Brute Force 사용 상황

입력으로 주어지는 데이터(N)의 수가 작으며 제한되어 있어야한다,

## Brute Force 사용 예시
### 선형 구조 - 순차적 탐색
![Desktop View](https://cdn-icons-png.flaticon.com/512/4305/4305535.png){: width="100" height="100" .w-20 .left}
<br>
아래의 코드는 단순히 4자리로 이루어진 자물쇠를 0부터 9999까지 직접 입력 해가며 푸는 알고리즘이다. 아래의 예시는
단순히 4자리로 이루어진 정수이지만 자릿수가 늘어나면 늘어날수록 정수 이외의 다른 문자를 허용할 수록 해당 문제의 시간복잡도는 기하급수적으로
증가한다.
<br>
```java
public class Locker {
    int password = 1234;

  public static void main(String[] args) {
    for(int i = 0 ; i < 9999 ; i++){
        if(i == password){
          System.out.println("password = " + i);
          break;
        }
    }
  }
}
```


### 비선형 구조 - DFS, BFS
TBU
