# 👻DOM
 <em> 문서 객체 모델 </em>  <br>
* 노드 트리 <br>
<img src=https://www.freecodecamp.org/news/content/images/size/w1000/2021/09/Document.jpg>
<br>

# 👻문서에서 요소를 선택하는 방법
## getElementById()
```
<p id="para1">This is my first paragraph.</p>
[console창]document.getElementById("para1")
const paragraph1 = document.getElementById("para1");
console.log(paragraph1);
```
<br>
<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Shot-2021-09-26-at-2.25.49-PM.png>
<br>

>단락의 내용만 읽으려는 경우 
`textContext`
```
const paragraph1 = document.getElementById("para1");
console.log(paragraph1.textContent);
```


<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Shot-2021-09-26-at-2.35.31-PM.png>

<br>

## querySelector()

```
<h1>Favorite TV shows</h1>
<ul class="list">
  <li>Golden Girls</li>
  <li>Archer</li>
  <li>Rick and Morty</li>
  <li>The Crown</li>
</ul>
```

<br>

```
[console창]const h1Element = document.querySelector("h1");
console.log(h1Element);
```

<br>

<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Shot-2021-09-26-at-3.15.59-PM.png>

```
const list = document.querySelector(".list");
console.log(list);
```

<br>

<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Shot-2021-09-26-at-3.22.45-PM.png>

### querySelectorAll()
```
const listItems = document.querySelectorAll("ul > li");
console.log(listItems); 
```
<br>
<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Shot-2021-09-26-at-3.30.46-PM.png>
