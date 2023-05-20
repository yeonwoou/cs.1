<h1> float</h1>
*원래 ‘뜨다’ 라는 의미이며, 원래 웹페이지에서 이미지를 어떻게 띄워서 텍스트와 함께 배치할 것인가에 대한 속성<br>
*float으로 컨텐츠를 띄울 시 다음 내용은 빈자리를 채우려 올라오게 된다.
<h1>클리어픽스(clearfix)</h1>
*float으로 인해 나타나는 요소들이 float속성에 영향을 더 이상 받지 않게함 
<br>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FmNmim%2FbtqYN2G10X2%2Fh4C482slaaIFpKVqTDzrSK%2Fimg.png">
```css
.clearfix:before, .clearfix:after {
    display: block;
    content: '';
    line-height: 0;
}
.clearfix:after {
    clear:both;
}```
<br>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbLskcs%2FbtqYZ53y8zc%2FHbH9dkOeUVOMQw8kua4jd0%2Fimg.png">
