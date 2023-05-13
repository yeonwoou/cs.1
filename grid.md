`그리드 나누기`
display:grid;<br>
grid-template-columns:100px 200px 100px;<br>
grid-template-rows:150px 200px; <br>
<br><br>
`유연한 크기 단위`<br>
display:grid;<br>
grid-template-columns:1fr 1fr 1fr;<br>
grid-template-rows:150px 200px; <br>
<br><br>
`반복되는 값을 한 번에 쓰기` <br>
display:grid;<br>
grid-template-columns:repeat(3,1fr);<br>
grid-template-rows:150px 200px;<br>
<br><br>
`최소,최대값으로 크기 정하기`<br>
display:grid;<br>
grid-template-columns:repeat(3,minmax(2oopx,1fr));<br>
grid-template-rows:150px 200px;<br>
<br><br>
`간격 넣기`<br>
display:grid;<br>
grid-template-columns:repeat(3,minmax(200px,1fr));<br>
grid-template-rows:150px 200px;<br>
gap:20px 10px;<br>
<br><br>

