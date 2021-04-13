## 이진 트리

- 이진 트리(binary tree) 정의
  1. 루트 노드를 중심으로 두 개의 서브 트리로 나뉘어진다.
  2. 나뉘어진 두 서브 트리도 모두 이진 트리이어야 한다.



- 노드가 위치할 수 있는 곳에 노드가 존재하지 않는다면, 공집합(empty set)노드가 존재하는 것으로 간주한다.



- 포화 이진 트리(Full Binary Tree)
  - 모든 레벨이 꽉 찬 이진 트리
- 완전 이진 트리(Complete Binary Tree)
  - **완전 이진 트리**란 마지막 레벨을 제외한 모든 레벨의 node가 완전히 채워져 있으며 마지막 레벨의 node들은 가능한 한 왼쪽부터 채워져 있는 구조를 말한다. 





## 이진 탐색 트리

- 이진 트리의 일종
- 즉 이진 트리에 **데이터의 저장 규칙**을 추가한 것
- 이진 탐색 트리에는 데이터를 저장하는 규칙이 존재하며 그 규칙은 특정 데이터의 위치를 찾는데 사용할 수 있다.
- 데이터 저장 규칙
  1. 이진 탐색 트리의 노드에 저장된 키(key)는 유일하다.
  2. 루트 노드의 키가 왼쪽 서브 투리를 구성하는 어떠한 노드의 키보다 크다.
  3. 루트 노드의 키가 오른쪽 서브 트리를 구성하는 어떠한 노드의 키보다 작다.
  4. 왼쪽과 오른쪽 서브 트리도 이진 탐색 트리이다.





- 단점 : 저장 순서에 따라 탐색의 성능에 큰 차이가 난다.

  --> 이러한 단점을 해결한 규형 잡힌 이진 트리가 나옴

  --> 트리는 노드를 균형 있게 가지는 것이 성능에 유리하기 때문에 기본 트리에서 변형된 B-트리, B+ 트리, R-트	  리, 레드 블랙 트리, AVL 트리 등 다양한 종류의 트리 자료구조가 있습니다.
  
  

탐색2는 아직 안함...









## Tree - from 바킹독 사이트

- 







## c++  -> 더 찾아보기!

- C++ STL에서는 tree container를 제공하지 않는다 --> tree를 사용하려는 이유에 따라 tree를 구현하거나 대체할 자료형이 달라짐

  

- Tree를 사용하는 이유

  1. mirror the problem using a tree-like structure
  2. container that has tree like access characteristics
     - [`std::map`](https://en.cppreference.com/w/cpp/container/map) (and [`std::multimap`](https://en.cppreference.com/w/cpp/container/multimap))
     - [`std::set`](https://en.cppreference.com/w/cpp/container/set) (and [`std::multiset`](https://en.cppreference.com/w/cpp/container/multiset))





- map의 자료구조는 "트리(tree)"입니다(정확하게 말하면 트리 자료구조 중의 하나인 "레드-블랙 트리(Red-Black tree)"입니다).
  - 레드 블랙 트리는 자가 균형 이진 탐색 트리로써 삽입과 삭제가 일어나는 경우에 자동으로 그 높이를 작게 유지하는 이진 탐색 트리입니다.
  - 따라서 트리에 n개의 원소가 있을 때 **O****(log n**)의 시간 복잡도로 삽입, 삭제, 검색을 할 수 있다.