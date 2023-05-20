## float
* 원래 ‘뜨다’ 라는 의미이며, 원래 웹페이지에서 이미지를 어떻게 띄워서 텍스트와 함께 배치할 것인가에 대한 속성<br>
* float으로 컨텐츠를 띄울 시 다음 내용은 빈자리를 채우려 올라오게 된다.
## 클리어픽스(clearfix)
* float으로 인해 나타나는 요소들이 float속성에 영향을 더 이상 받지 않게함 
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
}
```
<br>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbLskcs%2FbtqYZ53y8zc%2FHbH9dkOeUVOMQw8kua4jd0%2Fimg.png">

## CDN (Contents Delivery Network)

* CDN은 컨텐츠 전달 네트워크의 약자로 말 그대로, 컨텐츠를 전달하는 네트워크를 구성하는 것이다. 보통 웹사이트를 로딩할 때는 웹 서버에 HTTP 요청을 하여 리소스를 가져오지만 웹 서버가 아니라 현재 사용자가 접속한 위치에서 가장 가까운 서버에 리소스를 캐싱해놓고 보다 빠르게 가져오는 기법이다. 물론, CDN 네트워크를 구축하기 위해선 해당되는 지역의 ISP(인터넷 제공업체, Internet Service Provider), 네트워크 사업자, 이동통신 사업자에게 서버의 호스팅 비용을 지불해야 한다. 이렇게 네트워크를 구축하게 되면 정적 리소스를 더욱 빠른 속도로 서비스 할 수 있게 되는 것이다.

<br>
 장점

* 리소스를 캐싱해놓기 때문에 로딩속도가 빨라진다.
* 1개의 웹서버에서만 리소스를 가져오지 않기 때문에 서버의 부하가 줄어든다.
* 보통 1개의 도메인이 10개의 병렬연결을 허용하는데 CDN을 사용하면 병렬연결이 늘어난다.

<br>
 단점

* 서버를 구축하는 비용 때문에 돈이 더 많이 든다.
* 사용자가 해당되는 CDN을 막아놓으면 리소스 로딩이 막힌다.
* 배포과정이 다소 복잡해질 수 있다.
* 보통 CDN 서비스회사는 각 나라마다의 서버들을 구축해 놓지만, 자신의 나라에 없어서 해외 CDN을 사용하는 경우 더 느려질 수 있다.

