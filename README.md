# manual-algo
for me


### 알고리즘 유형

```
해시
정렬
완전탐색
깊이/너비 우선탐색(DFS/BFS)

스택/큐
힙(Heap)

탐욕법
동적계획법
이분탐색
그래프
```

### 깊이/너비 우선탐색(DFS/BFS)
```
1. 그래프  
2. 방문했던 지점 다시 체크해야됨(안하면 무한루프)  
3. 너비우선탐색은 가까운곳부터 진행  
4. 깊이우선탐색은 막히지 않을떄까지 진행  
5. 깊이우선탐색은 모든걸 다 돌아야할수도있음  
6. 너비우선탐색은 모두 다 돌필요가 없음  
7. 깊이우선탐색보다는 너비우선탐색이 빠름    
8. 너비우선탐색은 최단거리 등 확인에 유효함  
9. 깊이우선탐색은 스택을 사용, 너비우선탐색은 큐를 사용  

노드 생성시  
marked를 추가한다.  

함수생성시(BFS,DFS)  
1. 큐와 스택을 각각 넣는다  
2. marked를 체크해서 방문여부를 확인후 출력한다.  


DFS의 경우
1. 스택에 넣는다
2. 스택에서 뺸다.
3. 출력한다.
4. 자식노드를 스택에 넣는다
```


### 완전탐색
모든 경우의수를 다 고려해서, 시간은 최대로 걸림  
예시 : 비밀번호 4자리 다 입력하기  
```
Brute Force  
비트마스크  
순열  
백트래킹  
BFS  
```


### JAVA
1. list를 array로
```
    ArrayList<Integer> list = new ArrayList<>();
    return list.stream().mapToInt(i -> i.intValue()).toArray();
    
    ArrayList<Integer> list = new ArrayList<>();
    int[] answer = new int[arrayList.size()];
    int p = 0;
    for(int value : arrayList) {
      answer[p++] = value;
    }
```
2. 3항비교, 세항 비교
```
        int maxScore = Math.max(score[0], Math.max(score[1], score[2]));
        
        if (person_1_point >= person_2_point && person_1_point >= person_3_point) {
            max = person_1_point;
        } else if (person_2_point >= person_1_point && person_2_point >= person_3_point) {
            max = person_2_point;
        } else {
            max = person_3_point;
        }
```
