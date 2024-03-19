﻿# 섯다 게임
###### Member. 김정렬, 김재윤, 박미람, 소성민

<br/>
<br/>

### 섯다 흐름도
> [!TIP]
> 🟠 - start, end
>
> 🟩 - console 출력
> 
> 🟦 - 조건문
> 
> 🟨 - 실행

![Java-12](https://github.com/encore-full-stack-5/gambling-git/assets/125454927/06ca4a38-316f-4463-8ea8-dba1b3f12c2d)

<br/>

### UML
![스크린샷 2024-03-19 오후 12 29 28](https://github.com/encore-full-stack-5/gambling-git/assets/125454927/da8dfa5f-e014-4006-8bc4-48d6252ef642)

<br/>

### 코드 간단설명

> **카드 분배**
> 
![Java-13 (2)](https://github.com/encore-full-stack-5/gambling-git/assets/125454927/a621febd-4e05-4c46-94fa-eb5b0b601371)
#### makeCard( ) - 카드 20장 만들기
#### draw( ) - List에 카드 4장 뽑기(랜덤, 중복제거)
#### pickMyCardList( ), pickComputerCardList( ) - 나/컴퓨터에게 draw()로 뽑은 카드 2장씩 분배

<br/>

> **점수 계산**
> 
![Java-13 (1)](https://github.com/encore-full-stack-5/gambling-git/assets/125454927/c255577b-2370-47d4-9b4f-1edfb7f905ed)
#### start( ) - 카드 조합 점수 (Integer)
#### startResult( ) - 카드 조합 결과 (String)

<br/>

> **점수**
> 
![Java-14 (1)](https://github.com/encore-full-stack-5/gambling-git/assets/125454927/1fdf1db2-92de-42c7-abf8-d93df397a9c9)

<br/>

> **특수 족보 조건**
> 
![Java-14 (2)](https://github.com/encore-full-stack-5/gambling-git/assets/125454927/74223093-b82a-4df2-a289-82cab0023416)

<br/>

**버그 모음**
<br/>
1️⃣ (나)삼팔광땡, (컴퓨터)아무거나 출력 -> 컴퓨터 값이 무조건 1끗으로 나오고, 패배했습니다!로 출력됨
<br/>
2️⃣ 멍구사/파토/무승부 -> 재경기 -> 결과 확인 -> 1. 게임 종료 선택 -> 종료되지 않음
<br/>
3️⃣ 게임 시작 -> 결과 확인 -> 0. 재경기 -> 결과 확인 -> 1. 게임 종료 -> 종료되지 않음
<br/>
<br/>
**추후 하고 싶은 것**
<br/>
1️⃣ 위 버그들 수정
<br/>
2️⃣ 회원/로그인 만들기 (DB활용)
<br/>
3️⃣ 유저들에게 돈(게임머니) 지급 -> 게임을 통해 돈+-
<br/>
4️⃣ 유저VS컴퓨터가 아닌 PVP로 플레이 (PVP를 할 수 없어도 구현)
<br/>
5️⃣ 스레드 활용 (ex. (멍구사/파토/무승부) 재경기 시작 전 2~3초 대기)


<br/>
<br/>
<br/>

### 회고
> **김정렬** : 이번 프로젝트는 3/11~ 3/19일 까지 진행한 섯다 게임 만들기 프로젝트였습니다.
섯다라는 게임의 진행방식이 굉장히 독특해서 각 조합별 결과를 어떻게 비교해서 출력해야 할지에 대한 고민과 그 조합들을 코드로 작성했을 때 코드의 진행 순서가 중요하다는 것 과 코드가 길어질 때 언제 누가 봐도 코드를 쉽게 읽을 수 있도록 간단한 주석 처리가 중요하다는 것과 차후 수정 및 변경에 대한 확장성에 대한 고민을 하게 된 프로젝트 였습니다.


> **김재윤** : 처음으로 참여한 프로젝트임에도 팀원들이 너무 잘 이끌어줘서 감사했고
자바 기초만 공부하다가 섯다라는 게임을 자바 코드로 구상하기 위해 로직이 생성되는 과정을 직접 체험하면서 이론들을 활용하고 구체화 시키는 과정이 어떻게 진행되고 얼마나 중요한지 깨닫게 되는 시간이었습니다
앞으로 코딩 공부를 해가는 과정에 큰 원동력이 될 것 같은 감사한 프로젝트였습니다.


> **박미람** : 프로젝트를 통해서 코드에 대한 재미와 팀원들과 함께 하는 재미를 느꼈습니다^^*


> **소성민** : 섯다라는 실제 구현화된 아이템을 JAVA로 구현을 하면 20가지 패로 만드는 조합 우선순위 알고리즘 및 SOILD 원칙 적용으로 interface imp 클래스 사용 공부를 김재윤, 김정렬, 박미람 함께 하여 좋았습니다.
