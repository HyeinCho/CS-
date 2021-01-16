## Tree

- 트리란 정점과 간선을 이용해 사이클을 이루지 않도록 구성한 그래프의 특수한 형태로, 계층이 있는 데이터를 표현하기에 적합하다.

- DAG(방향성이 있는 비순환 그래프)의 한 종류

- 구성요소:
  - Node (노드) : 트리를 구성하고 있는 각각의 요소를 의미
  - Edge (간선) : 트리를 구성하기 위해 노드와 노드를 연결하는 선
  - Root Node : 최상위에 있는 노드
  - Terminal Node(=leaf node, 단말노드) : 하위에 다른 노드가 연결되어 있지 않은 노드
  - Internal Node(내부노드, 비단말노드) : 단말노드를 제외한 모든 노드(루트 노드 포함)

 

### Binary Tree

- 각 노드가 최대 두 개의 자식을 갖는 트리

- 이진 트리 순회
  - 중위순회: 왼쪽 노드 -> 현재 노드 -> 오른쪽 노드
  - 전위순회: 현재 노드 -> 왼쪽 노드 -> 오른쪽 노드
  - 후위순회: 왼쪽 노드 -> 오른쪽 노드 -> 현재 노드

 

### Full Binary Tree VS Complete Binary Tree

- Full Binary Tree(정 이진 트리) : 모든 노드가 0개 또는 2개의 자식 노드만 갖는 이진 트리
- ![img](Tree.assets/clip_image002-1610710779061.jpg)
- Complete Binary Tree(완전이진트리) : 위에서 아래로, 왼쪽에서 오른쪽으로 순서대로 차곡차곡 채워진 이진 트리



### BST(Binary Search Tree)

- 효율적인 탐색을 위한 저장방법
- 규칙
  - 이진 탐색 트리의 노드에 저장된 키는 유일하다
  - 부모의 키가 왼쪽 자식 노드의 키보다 크다
  - 부모의 키가 오른쪽 자식 노드의 키보다 작다
  - 왼쪽과 오른쪽 서브트리도 이진 탐색 트리이다.
- 시간복잡도: O(log n), 정말 안좋은 경우에는 O(n)
  - 배열보다 많은 메모리를 사용 -> 시간복잡도가 O(n)으로 같게 되는 비효율적 상황 발생
  - 균형을 잡기 위한 트리 구조 재조정인 Rebalancing 기법이 등장
  - Red-Black Tree, AVL 트리 (O(logN) 시간에 insert와 find를 할 수 있을 정도로 균형이 잘 잡혀 있는 경우)

 

### Tree 관련 면접 질문

- BST와 BinaryTree에 대해 설명하세요
- B트리에 대해 설명하세요
 

 

#### 출처

https://github.com/JaeYeopHan/Interview_Question_for_Beginner/tree/master/DataStructure

https://gmlwjd9405.github.io/2018/08/12/data-structure-tree.html

 
