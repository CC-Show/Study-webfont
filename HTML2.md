# 두번째 장  HTML

이번 시간에는 전 시간에 배웠던 태그들에 이어 더 다양한 태그들을 알아보도록 하겠습니다!

준비물 : vs Code 등의 에디터



1. `<pre >`

`<pre> ` 태그는 HTML 코드를 입력한 그대로 보여주는 태그입니다. 먼저 아래 예시를 따라해 보세요

```html
<body>
hell           o,
world!
</body>
```

위 예제를 코드에 적고 브라우저에서 열면 `hell o, world!` 와 같이 코드상에서 쓴 개행(엔터)과 스페이스 등이 적용되지 않습니다.

그래서 위 코드처럼 적용되게 하려면 `<pre>` 태그를 사용할 수 있습니다.



```html
<body>
    <pre>
    hell             o,
    world!
    </pre>
</body>
```

이제 브라우저에서 정상적으로 출력이 되나 확인해보세요!



2. `<code>`

다음으로는, 위 `<pre>` 태그와 비슷한 태그를 설명하도록 하겠습니다. `<code>` 태그는 화면상에서 컴퓨터 코드를 출력할 수 있게 해줍니다. 다음 예제를 따라해보세요

```html
<body>
    normal text
    <br/>
    <code>computer text</code>
</body>
```

어떤가요? 그냥 텍스트와 `<code>` 태그를 이용한 텍스트에 차이가 있죠?



3. `<iframe>`

`<iframe>` 태그는 HTML 문서 안에 다른 문서를 틀을 사용하여 내장시킬 수 있습니다. 이것도 예제로 만나볼까요?

```html
<body>
   <iframe src = "http://www.ccshow.co.kr"></iframe>
</body>
```

작은 틀 안에 ccshow 사이트가 보이시나요? 이렇게 src 에 링크를 걸어주면 그 페이지를 틀 안에서 띄워줄 수 있게 됩니다.



4. `<small>`

`<small>` 태그는 작은 텍스트를 보여주는 태그입니다. 흔히 웹 사이트나, 작품들을 볼때면 밑에 copyright 가 써있는 경우를 종종 보실 수 있으실 겁니다. 다음 예제를 따라해보세요

```html
<body>
    <p>Hello CCShow!</p>
    <p><small>copyright 2017 by Pinnacle</small></p>
</body>
```

`<small>` 태그를 사용하면 자신의 copyright 를 좀 더 멋지게 표현할 수 있습니다!



5. `<strike>`

`<strike>` 태그는 흔히 텍스트에서 '취소선' 을 표시할 때 많이 사용합니다. 

```html
<body>
    <p><strike>저녁을 방금먹었지만 </strike>나는 배고프다</p>
</body>
```

위의 `<strike>` 태그를 사용하면 저녁을 방금먹었지만 에는 취소선이 그려집니다.



6. `<sub>`, `<sup>` 

위의 태그들은 텍스트의 중간 선에 맞춰서 위, 아래로 표현할 때 쓰입니다. 쉽게 말해 윗첨자, 아랫첨자라고도 할 수 있을것 같습니다.

```html
<body>
    <p>hey look up! <sup>I am here!</sup></p>
    <p>hey look down! <sub>I am Here!</sub></p>
</body>
```



7. `<mark>` 

우리는 중요한 단어나, 문장등을 보면 형광펜으로 표시를 해놓습니다. 이와 비슷하게 html 태그 중에서도 형광펜같이 표시를 할 수 있는 태그가 있습니다

```html
<body>
    <p>이 문장은 중요한 문장이 아니지만, 이 <mark>단어</mark>만큼은 중요하다.</p>
</body>
```

이쁘게 색칠이 되는것을 볼 수 있습니다! css 를 이용해서 형광펜의 색깔도 바꿀 수 있으니 참고하시기 바랍니다.



8. `<select>`

`<select>` 태그는 드롭다운 메뉴를 만들어 줍니다. `<option>` 태그를 같이 사용합니다.

```html
<select>
  <option>한놈</option>
  <option>두시기</option>
  <option>석삼</option>
  <option>너구리</option>
</select>
```

9. `<br/>`

1번 태그와 같이 코드상에서 그냥 개행을 해도 웹 브라우저에서는 적용이 안되는 모습을 볼 수 있었습니다. 그러면  `<pre>` 태그를 쓰지 않고 오직 '개행' 만 하려면 어떻게 해야 할까요?

```html
<body>
    hello<br/> my <br/> name <br/> is <br/> babo
</body>
```

이렇게 하면

```
hello
my
name
is
babo
```

와 같이 출력되는 것을 볼 수 있습니다.



10. `<audio>`

우리는 음악을 좋아합니다! 그래서 자신의 웹페이지에도 음악을 넣고 싶습니다. 그러기 위해서는 `<audio>` 태그를 사용하면 됩니다! 먼저, 자신이 사용할 음악을 다운받고, 폴더 안에 같이 위치하게 한다음, 다음 예제를 진행해보세요

```html
<audio controls="controls">
    <source src="애국가.mp3" type="audio/mp3" />
    <source src="애국가.ogg" type="audio/ogg" />
</audio>
```

이렇게 자신이 추가하고싶은 음악을 `<audio>` 태그를 사용하여 추가 할 수도 있습니다!!



오늘의 태그 설명은 여기서 마치도록 하겠습니다. 이 외에도 재미있는 태그들이 많이 있으니, 구글에 

html tag 라고 검색하여 찾아보시면 더욱 좋을 것 같습니다!