# inline
- display 속성이 inline으로 지정된 엘리먼트는 전후 줄바꿈 없이 한 줄에 다른 엘리먼트들과 나란히 배치된다.

- 대표적인 inline 엘리먼트로 &lt;span&gt;이나 &lt;a&gt;, &lt;em&gt; 태그 등을 들 수 있다.

- 예를 들어, 여러 개의 inline 엘리먼트로 다음과 같이 마크업하면 줄바꿈 없이 순서대로 한 줄에 보이게 된다.

```
before
<a>A</a>
<span>SPAN</span>
<em>EM</em>
after
```
- inline 엘리먼트를 사용할 때 주의할 점은, width와 height 속성을 지정해도 무시된다는 점이다. 왜냐하면 해당 태그가 마크업하고 있는 컨텐츠의 크기 만큼만 공간을 차지하도록 되어 있기 때문이다. 또한, margin과 padding 속성은 좌우 간격만 반영이 되고, 상하 간격은 반영이 되지 않는다.

요약 : display 속성이 inline으로 지정된 엘리먼트는 줄바꿈 없이 순서대로 한 줄에 배치되고, width, height 속성은 지정해도 무시되고, margin과 padding 속성은 좌우 간격만 반영이 된다.

# block
- display속성이 block으로 지정된 엘리먼트는 전후 줄바꿈이 들어가 다른 엘리먼트들을 밀어내고 혼자 한 줄을 차지한다.

- 대표적인 block엘리먼트로 &lt;div&gt;나 &lt;p&gt;,&lt;h1&gt;태그 등을 들 수 있다.

- 예를 들어 여러 개의 block 엘리먼트를 다음과 같이 마크업하면 매번 줄바꿈 되어 여러 줄에 보이게 된다.
```
before
<h1>H1</h1>
<div>DIV</div>
<p>P</p>
after
```
- block 엘리먼트는 inline 엘리먼트와 달리 width, height, margin, padding 속성이 모두 반영된다.

요약 : display 속성이 block 으로 지정된 엘리먼트는 전후 줄바꿈이 들어가고, width, height, margin, padding 속성이 모두 반영된다.

# inline-block
- display 속성이 inline-block으로 지정된 엘리먼트는 마치 하이브리드 모드처럼 동작한다. inline 엘리먼트처럼 줄바꿈 없이 한 줄에 다른 엘리먼트들과 나란히 배치되지만, block 엘리먼트처럼 width, height의 속성 지정 및 margin, padding 속성의 상하 간격 지정이 가능하다.

- 대표적인 inline-block 엘리먼트로 &lt;button&gt;이나&lt;input&gt;,&lt;select&gt;태그 등을 들 수 있다.

```
display: inline-block;
```
inline-block 엘리먼트는 위와 같이 명시적으로 해당 엘리먼트의 스타일을 지정해줘야 한다.

- inline-block을 이용하면 여러 개의 엘리먼트를 한 줄에 정확히 원하는 너비만큼 배치할 수 있기 때문에 레이아웃에 활용 가능하다.

요약 : display 속성이 inline-block으로 지정된 엘리먼트는 내부적으로는 block 엘리먼트의 규칙을 따르면서 외부적으로 inline 엘리먼트의 규칙을 따른다. 스타일을 지정해줘야 한다.

