# flex
#### Flex 레이아웃을 만들기 위한 기본적인 HTML 구조는 다음과 같다.
```
<div class="container">
	<div class="item">helloflex</div>
	<div class="item">abc</div>
	<div class="item">helloflex</div>
</div>
```
- 부모 요소인 div.container를 Flex Container(플렉스 컨테이너)라고 부르고,
자식 요소인 div.item들을 Flex Item(플렉스 아이템)이라고 부른다.

- “컨테이너가 Flex의 영향을 받는 전체 공간이고, 설정된 속성에 따라 각각의 아이템들이 어떤 형태로 배치되는 것”이라고 생각하면 된다.

# flex의 속성
- 컨테이너에 적용하는 속성
- 아이템에 적용하는 속성

이렇게 두 가지로 나뉜다.

## flex 컨테이너에 적용하는 속성들
#### display : flex ;
```
.container {
	display: flex;
	/* display: inline-flex; */
}
```
- flex 아이템들은 가로 방향으로 배치되고, 자신이 가진 내용물의 width 만큼만 차지하게 된다. height는 컨테이너의 높이만큼 늘어난다.(정렬 속성을 통해 height를 어떻게 처리할지 조정 가능)

- inline-flex는 inline-block처럼 동작한다.
