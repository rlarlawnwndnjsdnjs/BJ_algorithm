# Algorithm
여기는 백준 문제!

1. BJ_2961.java 백준2961번 도영이가 만든 맛있는 음식(실버1)
-부분집합과 재귀를 사용하여 문제를 해결하였다.

2. Prob_7.java 백준15815번 천재 수학자 성필(실버4)
-스택과 스위치문을 사용하여 문제를 해결하였다.

3. BJ_1244.java 백준1244번 스위치 켜고 끄기(실버3)
-간단한 구현 문제였다. 하지만 각 위치의 스위치 값을 비교하여 같으면 스위치 상태를 변경하고 다르면 반복문을 탈출하는 라인(60~73)에서 런타임에러(ArrayIndexOutOfBounds)라는 결과가 떠서 이를 해결하는데 시간이 좀 들었다.

4. BJ_11724.java 백준11724번 연결 요소의 개수(실버2)
-dfs에 대해서 이해를 하고 문제를 몇 개 풀어본 후 dfs와 함께 배웠던 bfs에 대해서도 구현을 해보고 싶어 문제를 풀었고, dfs와 다르게 bfs는 큐를 이용해서 인접한 노드들을 큐에 넣고 하나씩 빼며, 빼낸 노드의 인접한 노드를 다시 넣고를 반복하는 작업을 통해 문제를 해결해 나가는 방법이었다. 이 문제에서는 연결 요소의 개수를 구하는 문제였기 때문에 첫 번째 노드부터 들어가서 인접한 노드들을 모두 큐에 넣고 방문처리를 해주고 모두 빼준다. 그렇게 해서 bfs메서드가 끝나게 되면 연결 요소의 개수를 1 증가시켜주고 다음 노드를 주며 bfs를 반복하는 방법을 통해 문제를 풀었다. 아직 완전히 이해하지 못했고, 추가적인 문제들을 풀어야한다.

5. BJ_1260.java 백준1260번 DFS와 BFS(실버2)
-이때까지 배우고 공부했던 dfs와 bfs에 대해서 확인해보는 문제였다. 좋은 복습 문제였고, bfs는 조금 더 공부해서 마스터하자.

6. BJ_1759.java 백준1759번 암호 만들기(골드5)
-이번 문제는 조합을 사용하여 풀었다. 기본 조합과 비슷한 로직을 구현했고 추가적인 조건(최소 한개의 모음, 최소 두개의 자음)을 설정해주었는데 입력받은 배열에서 모음을 찾으면 count1을 1올려주고, 자음을 찾으면 count2를 1올려준다. 그렇게 해서 count1이 1 이상이고 count2가 2 이상이면 출력되게 코드를 작성하였다.

7. BJ_10026.java 백준10026번 적록색약(골드5)
-dfs를 사용하여 해당하는 연결되어 있는 색의 지역을 모두 방문 후 지역 수를 1 올려주었다. 적록색약인 상태에서 봤을 때는 Red와 Green이 같은 색으로 보이기 때문에 Green을 Red로 만들어준후 다시 dfs를 돌려 지역 수를 찾아주었다.

8. BJ_1789.java 백준1789번 수들의 합(실버5)
-그리디 알고리즘으로 분류된 문제이다. 서로 다른 N개의 자연수의 합이 S인데 S가 주어졌을 때 자연수 N의 최대값을 구하는 문제이다. 그리디 알고리즘은 머릿속으로 문제를 직관적으로 해결할 때와 흡사하다. 1부터 숫자들을 더해가면서 마지막에 숫자를 더했을 때 S보다 커진다면 마지막 숫자를 빼고 S에 맞는 숫자를 더해주면 된다. 간단하게 해결한 문제이다.

9. BJ_2217.java 백준2217번 로프(실버4)
-그리디 알고리즘으로 해결할 수 있는 문제이다. 로프의 개수를 받고 N개의 로프로 물건을 든다 했을 때 N개의 로프 중 들 수 있는 최소 무게를 N개 로프만큼 곱하면 들 수 있는 최대의 무게가 된다. 이를 이용하여 for문을 사용하여 N개의 로프를 선택했을 때 들 수 있는 무게의 최대값을 갱신시킨 후 최대값을 출력한다.

10. BJ_11720.java 백준11720번 숫자의 합(브론즈2)
-이 때까지 풀었던 문제들을 보다가 풀지 못한 문제들을 살펴보다가 왜 틀렸지 하는 마음에 다시 풀어보았다. 난이도를 보니 학교다닐때 풀어본 문제 같은데 왜 틀렸나 싶은 마음이 든다. N개의 숫자를 공백없이 입력받는 거에서 String으로 받아서 for문을 돌며 charAt()으로 하나씩 빼내서 sum변수에다가 더해주면 해결되는 문제이다.

11. BJ_5525.java 백준5525번 IOIOI(실버2)
-패턴 반복 횟수 N번 붙여서 하나의 패턴 문자열로 만들어서 전체 문자열과 비교하며 패턴 문자열과 일치하면 카운트해주는 코드를 작성했지만 50점이었다. 스터디원이 푼 방법을 보고 설명을 들어보니 문자열 비교는 패턴 문자열이 길어질수록 시간이 많이 걸린다고 했다. 그래서 IOI만으로 비교하면서 IOI가 일치할 때마다 카운트해주고 카운트가 N이 된다면 전체를 하나로 보고 결과값을 1올려주는 방식으로 코딩하여 해결하는 문제이다.

12. BJ_1012.java 백준 1012번 유기농 배추(실버2)
-완전탐색(dfs, bfs)을 완벽하게 짤 수 있도록 하기 위해 기초부터 다시 시작하기 위해 풀었다. 배추흰지렁이는 인근에 있는 모든 배추의 해충을 잡아먹을 수 있다. bfs를 이용하여 인근 배추를 확인하고 count++시킨다. 모든 배열을 확인하고 결과를 출력하게 했다.









