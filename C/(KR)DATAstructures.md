# C 자료구조
**데이터의 구조를 조작**  
26.9.14/ 9.16
## 선형 자료구조, 비선형 자료구조
### 선형 자료구조 
- 배열 (array) 
> 리스트, 연결 리스트 (linkedList) 

> 배열의 크기는 정해져 있는데, 요소를 예측하지 못함, 메모리의 비효율성  
> 배열(이름자체가 주소) 이름을 기준으로 데이터 요소를 삽입 

> 탐색(삽입)하기가 편하다  
> 배열의 구조를 이용하여 배열 내에 있는 데이터의 순서를 변경할 뿐이다.  
> 배열안에서는 정렬만

> 리스트(배열)은 공백을 허용하지 않는다.  
> 이러한 단점을 보완하는 자료구조 --> 연결리스트 (포인터,참조)  
> data|link --- data|link --- data|link ...  
> link _ 포인터 변수  
> {data|link} - Node (데이터의 저장 장소)  
> {요소(정수,실수,문자) | 주소 (정수)} 자기참조구조체

```
struct Node (
  data Type value;
  pointer *link;
)
```
> Node 에서 데이터를 가지고 있지 않고 단지 주소만 가질 수 있는 노드가 존재 00> header(Dummy) Node  

- 스택 (stack) 
- 큐 (queue) 
### 비선형 자료구조  
- 트리 
- 그래프 - linkedList 

> 선형 ---> 규칙이 존재 , 비선형 자료 -> 규칙이 존재  
> 비선형 자료구조는 구현이 어렵다

## 동적(malloc(), ArrayList) 자료구조, 정적(배열)자료구조 | 메모리 할당에 관한 관련된 관점
### 동적 자료구조
> 길이값 조절 가능
### 정적 자료구조
> 한번 선언하면 끝

_26.09.14 구조체, 포인터 복습_

## 구조체  
### 자기참조구조체와 외부참조구조체  
#### 외부참조 구조체  
``` c
struct point {
  int x;
  int y;
}

struct student {
  char name [15];
  struct point* p;
};

int main(void) {
  struct student std1 = {"Kim", NULL };
  struct student std2 = {"Lee", NULL };

  struct point p1 = {10,20};
  struct point p2 = {30,40};

  std1.p = &p1;
  std2.p = &p2;
};
```
-> : 포인터가 가리키는 구조체의 멤버에 접근  

## linkedList | 연결자료 구조
1. 노드의 구조    
  [ 요소 (data filed), 주소 ] 로 이루어진 단위 --> node    
  [data | link]    
  [ A | B* ] -> [B | C*] -> [C | NULL]    
  세개의 노드의 구조체 이름은 같다. (자기 참조 구조체)  
<img width="1950" height="1046" alt="KakaoTalk_20260916_204437506" src="https://github.com/user-attachments/assets/4f9fad2b-817a-4813-9ef4-af209a5d4acf" />   
노드의 구조체를 다음과 같이 정의할 수 있다.

자기참조구조체 
``` c
struct Node {
  char data[4];
  struct Node* link;
};
```

[week] ---> 헤더노드 (더미)  
: 실질적인 노드에 포함을 하지 않는다

### 연결 리스트에 새로운 노드를 삽입하는 순서
1. 삽입할 노드를 준비 (생성)
2. 새 노드의 데이터 필드에 값을 저장
3. 새 노드의 주소를 저장
4. 새롭게 삽입할 노드를 연결한다
