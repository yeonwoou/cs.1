# DOM
 <em> 문서 객체 모델 </em>  <br>
* 노드 트리 <br>
<img src=https://www.freecodecamp.org/news/content/images/size/w1000/2021/09/Document.jpg>
<br>

## 문서에서 요소를 선택하는 방법
+ getElementById()
```
<p id="para1">This is my first paragraph.</p>
[console창]document.getElementById("para1")
const paragraph1 = document.getElementById("para1");
console.log(paragraph1);
```
<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Sho
     t-2021-09-26-at-2.25.49-PM.png>
+ querySelector()
 ```
<h1>Favorite TV shows</h1>
<ul class="list">
  <li>Golden Girls</li>
  <li>Archer</li>
  <li>The Crown</li>
</ul>
[console창]const h1Element = document.querySelector("h1");
console.log(h1Element);
```
<img src=https://www.freecodecamp.org/news/content/images/2021/09/Screen-Shot-2021-09-26-at-3.15.59-PM.png>

+ querySelectorAll()
```
<p id ="para1"> this. </p>
[console창]document.getElementById("para1")
```
