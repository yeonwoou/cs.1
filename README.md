운영체제(OS)
역할
__1.입력과 출력장치__
__2.저장과 불러오기__
`저장장치의 종류`
휘발성[RAM];컴퓨터가 켜져 있는 동안에몬 보관 VS 비휘발성 하드리스크;컴퓨터가 꺼져도 저장
빠르고 작은 용량 vs느리고 많은 용량 데이터 수정 가능 VS 데이터 수정 불가능[ROM}
__3.멀티태스킹(여러 프로그램 동시에 빠르게 진행하기)__

종류

1.데스크톱/랩톱 ;Window MacOs Linux
2.모바일 ;Android IOS
3.서버(큰 컴퓨터): 안정성,속도,효율이 가장 중요!
4.임베디드 ATM,POSS,항공기,TV종류나 환경이 다양해서 운영체제 많음 실시간 운영체제(RTOS)정해진 시간 내에 동작

UNIX: 대부분 c언어로 작성,다른 컴퓨터에 수정해서 적용 쉬움 >POSIX: Unix라면 갖춰야 할 규격과 기능 (표준) GNU(GNU is not Unix):Unix의 코드를 한 줄도 사용하지 않고 만든 Unix와 유사한 OS
GNU+Linux Kernel=Linux
Linux:마음대로 변형 +반드시 코드 공개 =>수 많은 변형 운영 체제 등장
********
<h1>마진겹침 현상</h1><br><br>
마진겹침(Margin-Collapsing)이란?<br> 블록 레벨 엘리먼트(Block-level element)에 한해 발생하는 현상으로 좌우 방향으로는 적용되지 않고 **오로지 수직 방향**으로 적용된다.
2개의 마진이 겹칠 때 더 큰 마진으로 덮어씌우는 방식이며 하나의 마진이 음수일 경우 더하는 방식을 취한다.<br>
1.인접한 엘리먼트<br>
.element1 {margin-bottom:20px;}<br>
.element2 {margin-top:40px;}<br>
둘 사이의 간격은 40px
<br>
2.부모의 처음/마지막 자식에서<br>
.parent{margin-top:20px;}<br>
,child{margin-top:20px;}<br>
둘의 마진이 같기 때문에 20px이 된다.<br> 해결하기 위해서는 부모에 inline컨텐츠,border,padding을 줘서 경계를 구분시키면 된다.<br>
 .parent{margin-top:20px;
Border:1px solid red;}
<br>
3.빈 엘리먼트<br>
.empty{margin-top:50px;}<br>
.element{margin-top:100px;}<br>
높이가 없는 빈 엘리먼트가 인접해있을 때도 마진겹침이 발생해 위쪽 마진은 100px이 된다. <br>이를 해결하기 위해선 빈 엘리먼트에 height min-height,padding,border나 inline 컨텐츠를 줘서 경계를 구분시키면 된다.<br>
.empty{margin-top:50px;
border:1px solid red;}
