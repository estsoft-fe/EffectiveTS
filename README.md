# 이펙티브 타입스크립트

<p align="center">
    <img src="./image/main.png">
</p>

---

> 타입스크립트 동작원리의 이해와 구체적이 조언들을 책을 통해 이해한 후 해당 내용을 정리하기 위해 만든 기록지입니다.

<br>

## 1. Index

##### 01. 타입스크립트 알아보기

##### 02. 타입스크립트의 타입 시스템

##### 03. 타입 추론

##### 04. 타입 설계

##### 05. any 다루기

##### 06. 타입 선언과 @types

##### 07. 코드를 작성하고 실행하기

##### 08. 타입스크립트로 마이그레이션하기

<br>
<br>
<br>

## 2. Table (ToDo)

<!-- ```
Rule 😎
00. 목차 이름을 딴 브랜치를 만들고 브랜치로 별로 push를 한다.
01. 작성자를 뺴먹지 않고 작성한다.
02. 한 페이지의 정리가 끝나면 작은 제목의 내부 링크를 연결한다.
03. 페이지 경로는 contents/인덱스.목차이름/인덱스.큰제목/인덱스-숫자.작은 제목(없다면 생략).md (한글로 입력하기)
    * ex) contents/01.데이터타입/1.데이터타입의종류/1-1.데이터타입의종류.md

04. 작성 내용은 default 포맷을 참고하여 작성한다. (contents/default.md 참고)
05. 이미지 첨부시 경로는 image/인덱스.목차이름/.(png | jpeg | jpg)
    * ex) image/01.데이터타입/byte.jpeg

06. 작성이 끝난 후 README.md 파일에서 완료 여부에 체크를 한다.
```

<br>
<br> -->

**01장.타입스크립트 알아보기** 😜

| <center>아이템</center>      | <center>제목</center>                                   | <center>페이지</center> | <center>작성자</center> | <center>완료</center> |
| :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 1           | [타입스크립트와 자바스크립트의 관계이해하기][타입스크립트와 자바스크립트의 관계이해하기]                       |            2            |           |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 2           | [타입스크립트 설정 이해하기][타입스크립트 설정 이해하기]                       |            9            |           |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 3           | [코드 생성과 타입이 관계없음을 이해하기][코드 생성과 타입이 관계없음을 이해하기]                       |            13            |           |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 4           | [구조적 타이핑에 익숙해지기][구조적 타이핑에 익숙해지기]                       |            21            |           |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 5           | [any 타입 지양하기][any 타입 지양하기]                       |            27            |           |     |:-----------------------------:

<br>
<br>

**02장. 타입스크립트의 타입 시스템** 😝

| <center>아이템</center>      | <center>제목</center>                                   | <center>페이지</center> | <center>작성자</center> | <center>완료</center> |
| :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 6           | [편집기를 사용하여 타입 시스템 탐색하기][편집기를 사용하여 타입 시스템 탐색하기]                       |            33            |     [Sumin][sumin]      |  :heavy_check_mark:  | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 7           | [타입이 값들의 집합이라고 생각하기][타입이 값들의 집합이라고 생각하기]                       |            38            |     [Sumin][sumin]      |   :heavy_check_mark: |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 8           | [타입 공간과 값 공간의 심벌 구분하기][타입 공간과 값 공간의 심벌 구분하기]                       |            46            |     [KangHyen][kangHyen]      | :heavy_check_mark:   |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 9           | [타입 단언보다는 타입 선언을 사용하기][타입 단언보다는 타입 선언을 사용하기]                       |            53            |     [KangHyen][kangHyen]      |  :heavy_check_mark:  |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 10           | [객체 래퍼 타입 피하기][객체 래퍼 타입 피하기]                       |            57            |     [TaeHyen][taeHyen]      |  :heavy_check_mark:   |:-----------------------------:|
| 11           | [잉여 속성 체크의 한계 인지하기][잉여 속성 체크의 한계 인지하기]                       |            61            |     [TaeHyen][taeHyen]      |   :heavy_check_mark: | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 12           | [함수 표현식에 타입 적용하기][함수 표현식에 타입 적용하기]                       |            65            |     [Sangcho][sangcho]      |  :heavy_check_mark:  |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 13           | [타입과 인터페이스의 차이점 알기][타입과 인터페이스의 차이점 알기]                       |            69            |     [Sangcho][sangcho]      |   :heavy_check_mark: |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 14           | [타입 연산과 제너릭 사용으로 반복 줄이기][타입 연산과 제너릭 사용으로 반복 줄이기]                       |            75            |     [Sumin][sumin]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 15           | [동적 데이터에 인덱스 시그니처 사용하기][동적 데이터에 인덱스 시그니처 사용하기]                       |            84            |     [Sumin][sumin]      |     |:-----------------------------: |
| 16           | [number 인덱스 시그니처보다는 Array,튜플,ArrayLike를 사용하기][number 인덱스 시그니처보다는 Array,튜플,ArrayLike를 사용하기]                       |            89            |     [Sumin][sumin]      |    | :-----------------------------: | ------------------------------------------------------------ | |
| 17           | [변경 관련된 오류 방지를 위해 readonly 사용하기][변경 관련된 오류 방지를 위해 readonly 사용하기]                       |           93            |     [KangHyen][kangHyen]      |    | :-----------------------------: | ------------------------------------------------------------ | |
| 18          | [매핑된 타입을 사용하여 값을 동기화하기][매핑된 타입을 사용하여 값을 동기화하기]                       |           101            |     [KangHyen][kangHyen]      |    | :-----------------------------: | ------------------------------------------------------------ |

<br>
<br>

**03장. 타입 추론** 😋

| <center>아이템</center>      | <center>제목</center>                                   | <center>페이지</center> | <center>작성자</center> | <center>완료</center> |
| :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 19           | [추론 가능한 타입을 사용해 장황한 코드 방지하기][추론 가능한 타입을 사용해 장황한 코드 방지하기]                       |            108            |     [KangHyen][kangHyen]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 20           | [다른 타입에는 다른 변수 사용하기][다른 타입에는 다른 변수 사용하기]                       |            116            |     [TaeHyen][taeHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 21           | [타입 넓히기][타입 넓히기]                       |            118            |     [TaeHyen][taeHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 22           | [타입 좁히기][타입 좁히기]                       |            123            |     [TaeHyen][taeHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 23           | [한꺼번에 객체 생성하기][한꺼번에 객체 생성하기]                       |            127            |     [Sangcho][sangcho]      |  :heavy_check_mark:   |:-----------------------------:| ------------------------------------------------------------ | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 24           | [일관성 있는 별칭 사용하기][일관성 있는 별칭 사용하기]                       |            131            |     [Sangcho][sangcho]      |  :heavy_check_mark:  | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 25           | [비동기 코드에는 콜백 대신 async 함수 사용하기][비동기 코드에는 콜백 대신 async 함수 사용하기]                       |            136            |     [Sangcho][sangcho]      |  :heavy_check_mark:  |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 26           | [타입 추론에 문맥이 어떻게 사용되는지 이해하기][타입 추론에 문맥이 어떻게 사용되는지 이해하기]                       |            142            |     [Sumin][sumin]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 27           | [함수형 기법과 라이브러리로 타입 흐름 유지하기][함수형 기법과 라이브러리로 타입 흐름 유지하기]                       |            147            |     [Sumin][sumin]      |    |:-----------------------------: | ------------------------------------------------------------ |

<br>
<br>

**04장. 타입 설계** 🥹

| <center>아이템</center>      | <center>제목</center>                                   | <center>페이지</center> | <center>작성자</center> | <center>완료</center> |
| :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 28           | [유효한 상태만 표현하는 타입을 지향하기][유효한 상태만 표현하는 타입을 지향하기]                       |            156            |     [Sumin][sumin]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 29           | [사용할 때는 너그럽게 생성할 때는 엄격하게][사용할 때는 너그럽게 생성할 때는 엄격하게]                       |            162            |     [KangHyen][kangHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 30           | [문서에 타입 정보를 쓰지 않기][문서에 타입 정보를 쓰지 않기]                       |            166            |     [KangHyen][kangHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 31           | [타입 주변에 null값 배치하기][타입 주변에 null값 배치하기]                       |            169            |     [KangHyen][kangHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 32           | [유니온의 인터페이스보다는 인터페이스의 유니온을 사용하기][유니온의 인터페이스보다는 인터페이스의 유니온을 사용하기]                       |            173            |     [TaeHyen][taeHyen]      |     |:-----------------------------:| ------------------------------------------------------------ | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 33           | [string타입보다는 더 구체적인 타입 사용하기][string타입보다는 더 구체적인 타입 사용하기]                       |            178            |     [TaeHyen][taeHyen]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 34           | [부정확한 타입보다는 미완성 타입을 사용하기][부정확한 타입보다는 미완성 타입을 사용하기]                       |            183            |     [TaeHyen][taeHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 35           | [데이터가 아닌 API와 명세를 보고 타입 만들기][데이터가 아닌 API와 명세를 보고 타입 만들기]                       |            189            |     [Sangcho][sangcho]      |  :heavy_check_mark:  |:-----------------------------: | ------------------------------------------------------------ |
| 36           | [해당 분야의 용어로 타입 이름 짓기][해당 분야의 용어로 타입 이름 짓기]                       |            195            |     [Sangcho][sangcho]      | :heavy_check_mark:   |:-----------------------------: | ------------------------------------------------------------ |
| 37           | [공식 명칭에는 상표를 붙이기][공식 명칭에는 상표를 붙이기]                       |            198            |     [Sangcho][sangcho]      |  :heavy_check_mark:  |:-----------------------------: | ------------------------------------------------------------ |

<br>
<br>

**05장. any 다루기** 😕

| <center>아이템</center>      | <center>제목</center>                                   | <center>페이지</center> | <center>작성자</center> | <center>완료</center> |
| :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 38           | [any 타입은 가능한 한 좁은 범위에서만 사용하기][any 타입은 가능한 한 좁은 범위에서만 사용하기]                       |            203            |     [Sumin][sumin]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 39           | [any를 구체적으로 변형해서 사용하기][any를 구체적으로 변형해서 사용하기]                       |            206            |     [Sumin][sumin]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 40           | [함수 안으로 타입 단언문 감추기][함수 안으로 타입 단언문 감추기]                       |            209            |     [Sumin][sumin]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 41           | [any의 진화를 이해하기][any의 진화를 이해하기]                       |            212            |     [KangHyen][kangHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 42           | [모르는 타입의 값에는 any 대신 unknown을 사용하기][모르는 타입의 값에는 any 대신 unknown을 사용하기]                       |            216            |     [KangHyen][kangHyen]      |     |:-----------------------------:| ------------------------------------------------------------ | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 43           | [몽키 패치보다는 안전한 타입을 사용하기][몽키 패치보다는 안전한 타입을 사용하기]                       |            221            |     [KangHyen][kangHyen]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 44           | [타입 커버리지를 추적하여 타입 안전성 유지하기][타입 커버리지를 추적하여 타입 안전성 유지하기]                       |            224            |     [TaeHyen][taeHyen]      |    |:-----------------------------: |

<br>
<br>

**06장. 타입선언과 @types** 🥹

| <center>아이템</center>      | <center>제목</center>                                   | <center>페이지</center> | <center>작성자</center> | <center>완료</center> |
| :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 45           | [devDependencies에 typescript와 @types 추가하기][devDependencies에 typescript와 @types 추가하기]                       |           229            |     [TaeHyen][taeHyen]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 46           | [타입 선언과 관련된 세 가지 버전 이해하기][타입 선언과 관련된 세 가지 버전 이해하기]                       |            232            |     [TaeHyen][taeHyen]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 47           | [공개 API에 등장하는 모든 타입을 익스포트하기][공개 API에 등장하는 모든 타입을 익스포트하기]                       |            238            |     [Sangcho][sangcho]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 48           | [API 주석에 TSDoc 사용하기][API 주석에 TSDoc 사용하기]                       |            239            |     [Sangcho][sangcho]      |    |:-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 49           | [콜백에서 this에 대한 타입 제공하기][콜백에서 this에 대한 타입 제공하기]                       |            243            |     [Sangcho][sangcho]      |     |:-----------------------------:| ------------------------------------------------------------ | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 50           | [오버로딩 타입보다는 조건부 타입을 사용하기][오버로딩 타입보다는 조건부 타입을 사용하기]                       |            248            |     [Sumin][sumin]      |    | :-----------------------------: | ------------------------------------------------------------ | :---------------------: | :---------------------: | :-------------------: |
| 51           | [의존성 분리를 위해 미러 타입을 사용하기][의존성 분리를 위해 미러 타입을 사용하기]                       |            251            |     [Sumin][sumin]      |    |:-----------------------------: |:---------------------: | :---------------------: | :-------------------: |
| 52           | [테스팅 타입의 함정에 주의하기][테스팅 타입의 함정에 주의하기]                       |            253            |     [Sumin][sumin]      |    |:-----------------------------: |

<br>
<br>

## 3. Reference

- [이펙티브타입스크립트][effective-typescript]

[effective-typescript]: https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=273193135&start=slayer
[sangcho]: https://github.com/SangchoKim
[taeHyen]: https://github.com/rlaxogus0517
[kangHyen]: https://github.com/bebekh1216
[sumin]: https://github.com/ttumzzi
[타입스크립트와 자바스크립트의 관계이해하기]: ./contents/01.타입스크립트알아보기/1.타입스크립트와자바스크립트의관계이해하기.md
[타입스크립트 설정 이해하기]: ./contents/01.타입스크립트알아보기/2.타입스크립트설정이해하기.md
[코드 생성과 타입이 관계없음을 이해하기]: ./contents/01.타입스크립트알아보기/3.코드생성과타입이관계없음을이해하기.md
[구조적 타이핑에 익숙해지기]: ./contents/01.타입스크립트알아보기/4.구조적타이핑에익숙해지기.md
[any 타입 지양하기]: ./contents/01.타입스크립트알아보기/5.any타입지양하기.md
[편집기를 사용하여 타입 시스템 탐색하기]: ./contents/02.타입스크립트의타입시스템/6.편집기를사용하여타입시스템탐색하기.md
[타입이 값들의 집합이라고 생각하기]: ./contents/02.타입스크립트의타입시스템/7.타입이값들의집합이라고생각하기.md
[타입 공간과 값 공간의 심벌 구분하기]: ./contents/02.타입스크립트의타입시스템/8.타입공간과값공간의심벌구분하기.md
[타입 단언보다는 타입 선언을 사용하기]: ./contents/02.타입스크립트의타입시스템/9.타입단언보다는타입선언을사용하기.md
[객체 래퍼 타입 피하기]: ./contents/02.타입스크립트의타입시스템/10.객체래퍼타입피하기.md
[잉여 속성 체크의 한계 인지하기]: ./contents/02.타입스크립트의타입시스템/11.잉여속성체크의한계인지하기.md
[함수 표현식에 타입 적용하기]: ./contents/02.타입스크립트의타입시스템/12.함수표현식에타입적용하기.md
[타입과 인터페이스의 차이점 알기]: ./contents/02.타입스크립트의타입시스템/13.타입과인터페이스의차이점알기.md
[타입 연산과 제너릭 사용으로 반복 줄이기]: ./contents/02.타입스크립트의타입시스템/14.타입연산과제너릭사용으로반복줄이기.md
[동적 데이터에 인덱스 시그니처 사용하기]: ./contents/02.타입스크립트의타입시스템/15.동적데이터에인덱스시그니처사용하기.md
[number 인덱스 시그니처보다는 Array,튜플,ArrayLike를 사용하기]: ./contents/02.타입스크립트의타입시스템/16.number인덱스시그니처보다는Array,튜플,ArrayLike를사용하기.md
[변경 관련된 오류 방지를 위해 readonly 사용하기]: ./contents/02.타입스크립트의타입시스템/17.관련된오류방지를위해readonly사용하기.md
[매핑된 타입을 사용하여 값을 동기화하기]: ./contents/02.타입스크립트의타입시스템/18.매핑된타입을사용하여값을동기화하기.md
[추론 가능한 타입을 사용해 장황한 코드 방지하기]: ./contents/03.타입추론/19.추론가능한타입을사용해장황한코드방지하기.md
[다른 타입에는 다른 변수 사용하기]: ./contents/03.타입추론/20.다른타입에는다른변수사용하기.md
[타입 넓히기]: ./contents/03.타입추론/21.타입넓히기.md
[타입 좁히기]: ./contents/03.타입추론/22.타입좁히기.md
[한꺼번에 객체 생성하기]: ./contents/03.타입추론/23.한꺼번에객체생성하기.md
[일관성 있는 별칭 사용하기]: ./contents/03.타입추론/24.일관성있는별칭사용하기.md
[비동기 코드에는 콜백 대신 async 함수 사용하기]: ./contents/03.타입추론/25.비동기코드에는콜백대신async함수사용하기.md
[타입 추론에 문맥이 어떻게 사용되는지 이해하기]: ./contents/03.타입추론/26.타입추론에문맥이어떻게사용되는지이해하기.md
[함수형 기법과 라이브러리로 타입 흐름 유지하기]: ./contents/03.타입추론/27.함수형기법과라이브러리로타입흐름유지하기.md
[유효한 상태만 표현하는 타입을 지향하기]: ./contents/04.타입설계/28.유효한상태만표현하는타입을지향하기.md
[사용할 때는 너그럽게 생성할 때는 엄격하게]: ./contents/04.타입설계/29.사용할때는너그럽게생성할때는엄격하게.md
[문서에 타입 정보를 쓰지 않기]: ./contents/04.타입설계/30.문서에타입정보를쓰지않기.md
[타입 주변에 null값 배치하기]: ./contents/04.타입설계/31.타입주변에null값배치하기.md
[유니온의 인터페이스보다는 인터페이스의 유니온을 사용하기]: ./contents/04.타입설계/32.유니온의인터페이스보다는인터페이스의유니온을사용하기.md
[string타입보다는 더 구체적인 타입 사용하기]: ./contents/04.타입설계/33.string타입보다는더구체적인타입사용하기.md
[부정확한 타입보다는 미완성 타입을 사용하기]: ./contents/04.타입설계/34.부정확한타입보다는미완성타입을사용하기.md
[데이터가 아닌 API와 명세를 보고 타입 만들기]: ./contents/04.타입설계/35.데이터가아닌API와명세를보고타입만들기.md
[해당 분야의 용어로 타입 이름 짓기]: ./contents/04.타입설계/36.해당분야의용어로타입이름짓기.md
[공식 명칭에는 상표를 붙이기]: ./contents/04.타입설계/37.공식명칭에는상표를붙이기.md
[any 타입은 가능한 한 좁은 범위에서만 사용하기]: ./contents/05.any다루기/38.any타입은가능한한좁은범위에서만사용하기.md
[any를 구체적으로 변형해서 사용하기]: ./contents/05.any다루기/39.any를구체적으로변형해서사용하기.md
[함수 안으로 타입 단언문 감추기]: ./contents/05.any다루기/40.함수안으로타입단언문감추기.md
[any의 진화를 이해하기]: ./contents/05.any다루기/41.any의진화를이해하기.md
[모르는 타입의 값에는 any 대신 unknown을 사용하기]: ./contents/05.any다루기/42.모르는타입의값에는any대신unknown을사용하기.md
[몽키 패치보다는 안전한 타입을 사용하기]: ./contents/05.any다루기/43.몽키패치보다는안전한타입을사용하기.md
[타입 커버리지를 추적하여 타입 안전성 유지하기]: ./contents/05.any다루기/44.타입커버리지를추적하여타입안전성유지하기.md
[devDependencies에 typescript와 @types 추가하기]: ./contents/06.타입선언과@types/45.devDependencies에typescript와@types추가하기.md
[타입 선언과 관련된 세 가지 버전 이해하기]: ./contents/06.타입선언과@types/46.타입선언과관련된세가지버전이해하기.md
[공개 API에 등장하는 모든 타입을 익스포트하기]: ./contents/06.타입선언과@types/47.공개API에등장하는모든타입을익스포트하기.md
[API 주석에 TSDoc 사용하기]: ./contents/06.타입선언과@types/48.API주석에TSDoc사용하기.md
[콜백에서 this에 대한 타입 제공하기]: ./contents/06.타입선언과@types/49.콜백에서this에대한타입제공하기.md
[오버로딩 타입보다는 조건부 타입을 사용하기]: ./contents/06.타입선언과@types/50.오버로딩타입보다는조건부타입을사용하기.md
[의존성 분리를 위해 미러 타입을 사용하기]: ./contents/06.타입선언과@types/51.의존성분리를위해미러타입을사용하기.md
[테스팅 타입의 함정에 주의하기]: ./contents/06.타입선언과@types/52.테스팅타입의함정에주의하기.md
