# 인프런 '실습 UI 개발로 배워보는 순수 JS 와 VueJS 개발' 강좌 따라하기

> 강좌에서 제공하는 github repo 를 fork 해서 정리한 내용입니다.

## 둘러보기

0.  [들어가며](#0-들어가며)
1.  [브랜치 순서](#1-브랜치-순서)
2.  [VanillaJS](#2-vanillajs)
3.  [Vue.js](#3-vuejs)
4.  [Component](#4-component)

## 0. 들어가며

인프런의 '실습 UI 개발로 배워보는 순수 JS 와 VueJS 개발' 강좌를 들으면서 실습을 진행한 내용입니다.

강좌에서 제공한는 repo 를 fork 해서 실습한 내용을 추가했습니다.

## 1. 브랜치 순서

강좌 진생 순서별로 어떤 브랜치를 찾아가야 하는지 정리한 내용입니다.

1.  Lecture 5 - 순수 JS (MVC)/폴더 구조 : 1-vanilla/scafolding
2.  Lecture 6 - 검색폼/검색폼 구현 1 : 1-vanilla/controller
3.  Lecture 7 - 검색폼/검색폼 구현 2 : 1-vanilla/FormView1
4.  Lecture 8 - 검색폼/검색폼 구현 3 : 1-vanilla/FormView2
5.  Lecture 9 - 검색폼/검색폼 구현 4 (실습) : 1-vanilla/FormView3
6.  Lecture 11 - 검색결과/검색결과 구현 1 : 1-vanilla/FormView4
7.  Lecture 12 - 검색결과/검색결과 구현 2 : 1-vanilla/ResultView1
8. 	Lecture 13 - 검색결과/검색결과 구현 3 (실습) : 1-vanilla/ResultView2
9.  Lecture 15 - 탭/탭 구현 1 : 1-vanilla/ResultView3
10. Lecture 16 - 탭/탭 구현 2 : 1-vanilla/TabView1
11. Lecture 17 - 탭/탭 구현 3 (실습) : 1-vanilla/TabView2
12. Lecture 19 - 추천 검색어/추천 검색어 구현 1 : 1-vanilla/TabView3
13. Lecture 20 - 추천 검색어/추천 검색어 구현 2 : 1-vanilla/KeywordView1
14. Lecture 21 - 추천 검색어/추천 검색어 구현 3 (실습) : 1-vanilla/KeywordView2
15. Lecture 23 - 최근 검색어/최근 검색어 구현 1, 2 : 1-vanilla/KeywordView3
16. Lecture 24 - 최근 검색어/최근 검색어 구현 3 : 1-vanilla/HistoryView1
17. Lecture 25 - 최근 검색어/최근 검색어 구현 4 (실습) : 1-vanilla/HistoryView2
18. Lecture 27 - 최근 검색어/최근 검새어 구현 checkout : 1-vanilla/HistoryView3
19. Lecture 28 - 최근 검색어/최근 검색어 구현 5 (실습) : 1-vanilla/HistoryView4
20. Lecture 31 - Vue.js (MVVM)/vue.js 설치 : 2-vue/scafolding
21. Lecture 32 - 검색폼/검색폼 : 2-vue/install
22. Lecture 33 - 검색폼/검색폼 (실습) : 2-vue/Form1
23. Lecture 35 - 검색결과/검색결과 : 2-vue/Form2
24. Lecture 36 - 검색결과/검색결과 (실습) : 2-vue/Result1
25. Lecture 38 - 탭/탭 : 2-vue/Result2
26. Lecture 39 - 탭/탭 (실습) : 2-vue/Tab1  
27. Lecture 41 - 추천 검색어/추천 검색어 구현 : 2-vue/Tab2
28. Lecture 42 - 최근 검색어/최근 검색어 : 2-vue/Keyword
29. Lecture 43 - 최근 검색어/최근 검색어 (실습) : 2-vue/History1
30. Lecture 47 - 컴포넌트/FormComponent 구현 1 : 3-component/scafolding
31. Lecture 48 - 컴포넌트/FormComponent 구현 2 : 3-component/FormComponent1
32. Lecture 49 - 컴포넌트/ResultComponent 구현 : 3-component/FormComponent2
33. Lecture 50 - 컴포넌트/ListComponent 구현 1 : 3-component/ResultComponent
34. Lecture 51 - 컴포넌트/ListComponent 구현 2 : 3-component/ListComponent1
35. Lecture 52 - 컴포넌트/TabComponent 1 : 3-component/ListComponent2

## 2. VanillaJS

해당 브랜치의 주제를 정리했습니다.

1.  [scafolding](#1-1-vanilla/scafolding)
2.  [controller](#2-1-vanilla/controller)
3.  [FormView1](#3-1-vanilla/formview1)
4.  [FormView2](#4-1-vanilla/formview2)
5.  [FormView3](#5-1-vanilla/formview3)
6.  [FormView4](#6-1-vanilla/fromview4)
7.  [ResultView1](#7-1-vanilla/resultview1)
8.  [ResultView2](#8-1-vanilla/resultview2)
9.  [ResultView3](#9-1-vanilla/resultview3)
10. [TabView1](#10-1-vanilla/tabview1)
11. [TabView2](#11-1-vanilla/tabview2)
12. [TabView3](#12-1-vanilla/tabview3)
13. [KeywordView1](#13-1-vanilla/keywordview1)
14. [KeywordView2](#14-1-vanilla/keywordview2)
15. [KeywordView3](#15-1-vanilla/keywordview3)
16. [HistoryView1](#16-1-vanilla/historyview1)
17. [HistoryView2](#17-1-vanilla/historyview2)
18. [HistoryView3](#18-1-vanilla/historyview3)
19. [HistoryView4](#19-1-vanilla/historyview4)
20. [HistoryView5](#20-1-vanilla/historyview5)

### 1. 1-vanilla/scafolding

vanillaJS 로 MVC 패턴을 구현할 때 사용하는 폴더 구조

### 2. 1-vanilla/controller

`MainController.js` 모듈 작성 및 등록

* `console.log()` 로 정상 작동하는지 출력

크롬 61 버전 이상부터 ES6 의 module system 지원

### 3. 1-vanilla/FormView1

`FormView.js` 모듈 작성

* `View.js` 모듈을 상속 받아 작성
* `FormView.setup` 메소드 작성
  * 인자로 받은 form 엘리먼트 (`el`) 를 프로퍼티에 등록
  * form 엘리먼트 (`el`) 의 text input 엘리먼트 (`el.querySelector('[type=text]')`) 를 `inputEl` 프로퍼티에 등록
  * form 엘리먼트 (`el`) 의 reset button 엘리먼트 (`el.querySelector('[type=reset]')`) 를 `resetEl` 프로퍼티에 등록
  * `FormView.showResetBtn()` 메소드를 `false` 인자를 전달하면서 실행
* `FormView.showResetBtn` 메소드 작성
  * 인자 `show` 로 `Boolean` 값 받음, 기본값은 `true`
  * 등록되어 있는 `resetEl` 의 `style.display` 프로퍼티 (`this.resetEl.style.display`) 값을 변경
    * `show` 인자가 `true` 라면 `'block'`
    * `show` 인자가 `false` 라면 `'none'`

`FormView.js` 모듈을 `MainController.js` 모듈에 등록

* `MainController.js` 의 `init()` 메소드에서 `FormView.setup()` 메소드 실행
  * 인자로는 form 엘리먼트 (`document.querySelector('form')`) 전달

실행 결과 첫 로딩 화면에서 reset button 은 화면에 표시되지 않음

### 4. 1-vanilla/FormView2

`FormView.js` 모듈 업데이트

* `FormView.setup()` 메소드에서 `this.bindEvents()` 메소드 호출
* `FormView.bindEvents` 메소드 작성
  * `this` (form 엘리먼트) 에 `'submit'` 이벤트 리스터 작성 (`View.js` 모듈에서 상속받은 `this.on()` 메소드 사용)
    * `e.preventDefault()` 로 form 엘리먼트의 기본 이벤트 방지
    * 엔터키를 누르면 폼 전송을 위해 화면 갱신이 이루어지는 기본 이벤트
  * 등록되어 있는 `this.inputEl` 엘리먼트에 `keyup` 이벤트 리스너 작성 (기본 `addEventListener()` 메소드 사용)
    * `this.onKeyup()` 메소드 실행 (인자로 이벤트 객체 넘겨줌)
* `FormView.onKeyup` 메소드 작성
  * `this.showResetBtn()` 메소드 실행
    * 인자로 `this.inputEl.value.length` 전달
      * `value` 값이 없다면 `length` 가 `0` 이므로 `false`
      * `value` 값이 있다면 `length` 가 자연수이므로 `true`

### 5. 1-vanilla/FormView3

`FormView.js` 모듈의 `FormView.onKeyup` 메소드 업데이트

* 엔터 키 코드 (`13`) 를 `enter` 상수에 정의
* 입력한 키가 엔터 키인지 확인
  * 엔터 키가 아니면 `return` 으로 함수 종료
  * 엔터 키라면 `this.emit()` 메소드 실행 (`View.js` 모듈에서 상속받음)
    * `'@submit'` 이라는 커스텀 이벤트 발생시킴
    * `{ input: this.inputEl.value }` 객체를 `emit` 메소드의 두 번째 인자 (`data`) 로 전달

`MainController.js` 모듈 업데이트

* `init` 메소드에서 `FormView.setup()` 메소드를 호출한 후 메소드 체이닝으로 `on()` 메소드 실행
  * `FormView.setup` 메소드, `FormView.on` 메소드에서 `this` (`FormView` 객체 자신) 를 `return` 하기 때문에 가능
  * `on` 메소드는 `View.js` 모듈에게 상속받은 것
  * `'@submit'` 이벤트에 대한 리스너 작성
    * `MainController.js` 모듈 (화살표 함수에서 `this` 는 외부 함수의 맥락을 따름, 본래 `addEventListener` 의 callback 함수 안에서 `this` 는 이벤트가 발생한 DOM 엘리먼트임) 의 `this.onSubmit()` 메소드 실행
      * 인자로 `e.detail.input` 값 전달 (`FormView.js` 모듈의 `FormView.onKeyup` 메소드 내부에서 `'@submit'` 이벤트를 발생시킬 때 전달한 객체)
* `onSubmit` 메소드 작성
  * `console.log()` 로 결과 출력해서 확인

### 6. 1-vanilla/FormView4

`FormView.js` 모듈 업데이트

* `FormView.bindEvents` 메소드 업데이트 - 등록되어 있는 `this.resetEl` 엘리먼트에 `click` 이벤트 리스너 작성 (기본 `addEventListener()` 메소드 사용) - `this.onClickReset()` 메소드 실행
* `FormView.onClickReset` 메소드 작성
  * `this.emit()` 메소드 실행 (`View.js` 모듈에서 상속받음)
    * 인자로 `'@reset'` 전달 (`'@reset'` 이벤트 발생시킴) - `this.showResetBtn(false)` 메소드 실행 - 리셋 버튼 안 보이게 함
* `FormView.onKeyup` 메소드 업데이트 - `this.inputEl.value.length` 값이 존재하지 않는다면 (`0` 이라면) `this.emit('@reset')` 메소드 실행

`MainController.js` 모듈 업데이트

* `init` 메소드 업데이트 - `FormView.setup().on()` 메소드 체이닝에 `FormView.on()` 메소드 추가 - `'@reset'` 이벤트 감지 - `this.onResetForm()` 메소드 실행
* `onResetForm` 메소드 작성 - `console.log()` 로 결과 출력해서 확인

현재 reset 버튼은 `input[type=reset]` 이기 때문에 기본으로 클릭하면 `input[type=text]` 의 내용 삭제함

### 7. 1-vanilla/ResultView1

`index.html` 업데이트

* 검색 결과를 출력할 영역 작성 - `form` 태그 아래에 `div[class=content]` 태그 작성 - 내부에 `div[id=search-result]` 태그 작성

`ResultView.js` 모듈 작성

* `View.js` 모듈을 `import` 한 후 `Object.create(View)` 메소드로 `View.js` 모듈을 상속받은 `ResultView.js` 모듈 생성
* `ResultView.setup` 메소드 작성 - `el` 을 인자로 받아 `this.init(el)` 메소드 실행 (`View.js` 모듈에서 상속받음)
* `ResultView.render` 메소드 작성 - `data` 를 인자로 받음 (기본은 빈 배열) - `console.log()` 로 결과 확인 - `this.el.innerHTML` 에 삼항 연산자 할당 - `data.length` 에 따라 - `true` 이면 `this.getSearchResultHtml(data)` - `false` 이면 `'검색 결과가 없습니다.'`
* `ResultView.getSearchResultHtml` 메소드 작성 - `data` 를 인자로 받음 - `debugger` 를 사용해 Break Point 생성
* `export default ResultView` 구문으로 모듈 내보냄

`MainController.js` 모듈 업데이트

* 필요한 모듈 불러옴 - `import ResultView from '../views/ResultView.js'` - `import SearchModel from '../models/SearchModel.js'`
* `init` 메소드 업데이트 - `ResultView.setup()` 메소드 실행 - `document.querySelector('#search-result')` 를 인자로 넘겨줌 (검색 결과 출력할 엘리먼트)
* `onSubmit` 메소드 업데이트 - `this.search(input)` 메소드 실행
* `search` 메소드 작성 - `query` 를 인자로 받음 - 검색어를 받는 인자 - `console.log()` 로 결과 확인 - `SearchModel.list(query)` 로 검색 결과 조회 - `Promise` 반환 - `then()` 메소드로 비동기 처리 - 반환한 `data` 를 받아 `this.onSearchResult(data)` 메소드 실행
* `onSearchResult` 메소드 작성 - `ResultView.render(data)` 메소드 실행

### 8. 1-vanilla/ResultView2

`ResultView.js` 모듈 업데이트

* `ResultView.getSearchResultsHtml` 메소드 업데이트 - 인자로 받은 `data` 를 `reduce()` 메소드로 가공하여 그 결과를 `return` 함 - 각 `item` 을 `this.getSearchItemHtml()` 메소드로 가공하여 그 결과를 `<ul></ul>` 태그 사이에 작성
* `ResultView.getSearchItemHtml` 메소드 작성 - `item` 을 인자로 받음 (상품 목록 하나) - `<li></li>` 태그 안에 `<img>` 태그와 상품 이름을 출력하는 `<p></p>` 태그 작성해서 `return`

### 9. 1-vanilla/ResultView3

`MainController.js` 모듈 업데이트

* `onResetForm` 메소드 업데이트
  * `ResultView.hide()` 메소드 실행
    * `ResultView.js` 모듈이 상속받은 `View.js` 모듈의 메소드
    * `this.el.style.display` 속성을 `'none'` 으로 변경

### 10. 1-vanilla/TabView1

`index.html` 파일 업데이트

* `div#search-result` 태그 위에 `ul` 태그 추가
  * `id` 와 `class` 속성에 모두 `tabs` 작성
  * 두 개의 `li` 태그 작성
    * 각각 '추천 검색어', '최근 검색어' 항목

### 11. 1-vanilla/TabView2

`TabView.js` 모듈 생성

* `View.js` 모듈 상속받아 생성
* `TabView.tabName` 프로퍼티 생성
  * 객체 할당
  * `recommand` 키에 `'추천 검색어'`
  * `recent` 키에 `'최근 검색어'`
* `TabView.setup` 메소드 작성
  * `el` 을 인자로 받아 `this.init(el)` 메소드 실행
  * `this.init()` 메소드는 `View.js` 모듈에서 상속받은 것
  * `this` 를 `return`
* `TabView.setActiveTab` 메소드 작성
  * `tabName` 을 인자로 받음
  * `Array.from(this.el.querySelectorAll('li'))` 로 `this.el` 아래의 모든 `li` 태그 선택하여 배열 생성
  * `.forEach(li => { ... })` 메소드로 각 `li` 의 className 변경
    * 만일 `li.innerHTML` 이 `tabName` 과 같다면 `'active'`
    * 만일 `li.innerHTML` 이 `tabName` 과 다르다면 `''`
  * `this.show()` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드

`MainController.js` 모듈 업데이트

* `TabView.js` 모듈 `import`
* `init` 메소드 업데이트
  * `TabView.setup()` 메소드 실행
    * `#tabs` 를 인자로 전달
  * `this.selectedTab` 에 기본값으로 `'추천 검색어'` 할당
  * `this.renderView()` 메소드 실행
* `renderView` 메소드 작성
  * `console.log` 로 디버깅
  * `TabView.setActiveTab()` 메소드 실행
    * 인자로 `this.selectedTab` 전달
  * `ResultView.hide()` 메소드 실행

### 12. 1-vanilla/TabView3

`TabView.js` 모듈 업데이트

* `TabView.setup` 메소드 업데이트
  * `this.bindClick()` 메소드 실행
* `TabView.bindClick` 메소드 작성
  * `Array.from(this.el.querySelectorAll('li')).forEach(li => { ... })` 로 `el` 아래 모든 `li` 태그를 순회
  * 각 `li` 태그마다 `addEventListener()` 메소드 실행
    * `'click'` 이벤트를 받음
    * `this.onClick()` 메소드 실행
      * 인자로 `li.innerHTML` 전달 (탭 이름)
* `TabView.onClick` 메소드 작성
  * `tabName` 을 인자로 받음
  * `this.setActiveTab(tabName)` 메소드 실행
  * `this.emit('@change', { tabName })` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드

`MainController.js` 모듈 업데이트

* `init` 메소드 업데이트
  * `TabView.setup()` 메소드 이후 메소드 체이닝으로 `.on('@change', e => { ... })` 메소드 실행
    * `on` 메소드는 `View.js` 모듈에서 상속받은 메소드
    * `e` 를 받아서 `this.onChangeTab(e.detail.tabName)` 메소드 실행
* `onChangeTab` 메소드 작성
  * `tabName` 을 인자로 받음
  * 디버깅을 위해 `console.log()` 로 출력

### 13. 1-vanilla/KeywordView1

`index.html` 업데이트

* `div#search-result` 태그 위에 `div#search-keyword` 태그 작성

`KeywordView.js` 모듈 작성

* `View.js` 모듈 상속
* `KeywordView.messages` 프로퍼티 작성
  * `NO_KEYWORDS` 프로퍼티에 `'추천 검색어가 없습니다'` 값 할당
* `KeywordView.setup` 메소드 작성
  * `el` 를 인자로 받음
  * `this.init(el)` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드
  * `this` 반환
* `KeywordView.render` 메소드 작성
  * `data = []` 를 인자로 받음
  * `this.el.innerHTML` 에 `data.length`에 따라 다른 값 할당
    * 길이가 있다면 `this.getKeywordHtml(data)`
    * 길이가 없다면 `this.messages.NO_KEYWORDS`
  * `this.show()` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드
* `KeywordView.getKeywordHtml` 메소드 작성
  * `data` 를 인자로 받음
  * `data.reduce( ... )` 로 생성한 HTML을 담은 문자열을 반환
  * 이때 `li` 태그에 `data-keyword` 속성으로 해당 아이템의 keyword 값 부여
  * 나중에 `(li element).dataset.keyword` 로 접근 가능
* `KeywordView` 를 `export`

`MainController.js` 모듈 업데이트

* `KeywordView.js`, `KeywordModel` 모듈 `import`
* `init` 메소드 업데이트
  * `KeywordView.setup(document.querySelector('#search-keyword'))` 메소드 실행
* `renderView` 메소드 업데이트
  * `this.selectedTab` 에 따라 분기
    * `'추천 검색어'` 일 경우 `this.fetchSearchKeyword()` 메소드 실행
    * 아닌 경우 `debugger`
* `fetchSearchKeyword` 메소드 작성
  * `KeywordModel.list()` 메소드로 데이터 가져옴
  * 프로미스 비동기 처리에 따라 결과를 `.then()` 메소드로 처리
    * `data` 를 받아서 `KeywordView.render(data)` 실행

### 14. 1-vanilla/KeywordView2

`KeywordView.js` 모듈 업데이트

* `KeywordView.render` 메소드 내부에서 `html` 을 랜더링 한 후 `this.bindClickEvent()` 메소드 호출
* `KeywordView.bindClickEvent` 메소드 작성
  * `this.el` 하위의 모든 `li` 태그에 대해 `click` 이벤트 리스너 작성
  * 이벤트 리스너 내부에서 `this.onClickKeyword(e)` 메소드 실행
    * 매개변수에 이벤트 객체 `e` 전달
* `KeywordView.onClickKeyword` 메소드 작성
  * `e.currentTarget.dataset.keyword` 로 해당 `keyword` 값 접근
  * `this.emit('@click', { keyword })` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드, 커스텀 이벤트 발행

`MainController.js` 모듈 업데이트

* `MainController.init` 메소드 업데이트
  * `KeywordView.setup( ... )` 메소드 호출 이후 메소드 체이닝으로 `.on()` 메소드 실행
    * `@click` 이벤트 수신
    * 이벤트 핸들러에서 `this.onClickKeyword()` 메소드 실행
      * `e.detail.keyword` 를 매개변수로 전달
        * 클릭한 리스트의 키워드 정보
* `MainController.onClickKeyword` 메소드 작성
  * `keyword` 를 매개변수로 받음
  * `this.search(keyword)` 메소드 실행
* `MainController.onSearchResult` 메소드 업데이트
  * `TabView.hide()` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드
  * `KeywordView.hide()` 메소드 실행
    * `View.js` 모듈에서 상속받은 메소드

### 15. 1-vanilla/KeywordView3

`MainController.js` 모듈 업데이트

* `MainController.search` 메소드 업데이트
  * `FormView.setValue(query)` 메소드 실행
    * `query` 는 현재 선택한 키워드
  * `MainController.onResetForm` 메소드 업데이트
    * `ResultView.hide()` 메소드 실행 대신 `this.renderView()` 메소드 실행

`FormView.js` 모듈 업데이트

* `FormView.setValue` 메소드 작성
  * `value` 를 인자로 받음
    * 기본값은 `''`
  * `this.inputEl.value` 에 인자로 받은 `value` 값 대입
  * `this.showResetBtn(this.inputEl.value.length)` 메소드 실행
    * 검색한 값이 있는 경우 취소 버튼을 보이게 하기 위함

### 16. 1-vanilla/HistoryView1

`index.html` 파일 업데이트

* `div[id="search-history"]` 태그 작성
  * `div[id="search-keyword"]` 태그 아래에 위치

`HistoryView.js` 모듈 Create

* `KeywordView.js` 모듈을 상속받음
  * `Object.create(KeywordView)` 메소드 사용
* `HistoryView` 모듈 export

`MainController.js` 모듈 Update

* `HistoryView.js` 모듈 import
* `HistoryModel.js` 모듈 import
* `init` 메소드 Update
  * `HistoryView` 설정
    * `KeywordView` 설정과 동일한 형식
    * `@click` 이벤트에 `onClickHistroy` 핸들러 등록
* `onClickHistory` 메소드 Create
  * `onClickKeyword` 메소드와 동일
* `renderView` 메소드 Update
  * 현재 탭이 '최근 검색어' 탭일 경우 `this.fetchSearchHistory()` 메소드 실행
* `fetchSearchHistory` 메소드 Create
  * `HistoryModel` 의 `list()` 메소드로 목록을 가져옴
  * `then` 으로 반환한 `Promise` 객체 처리
    * 받아온 `data` 를 `HistoryView.render(data)` 로 출력
      * `HistoryView` 의 `render` 메소드는 `KeywordView` 의 `render` 메소드를 상속받은 것

### 17. 1-vanilla/HistoryView2

`HistoryView.js` 모듈 Update

* `HistoryView.getKeywordsHtml` 메소드 Create
  * `KeywordView` 모듈의 `getKeywordsHtml` 메소드를 overriding
  * 최근 검색어를 보여줄 `ul` 태그와 내부의 `li` 태그를 문자열로 작성해 return

### 18. 1-vanilla/HistoryView3

`HistoryView.js` 모듈 Update

* `HistoryView.bindRemoveBtn` 메소드 Create
  * 해당 `el` 의 모든 `button.btn-remove` 에 `click` 이벤트에 대한 `eventListener` 를 연결
    * 이벤트 전파를 막음
    * `this.onRemove(btn.parentElement.dataset.keyword)` 메소드 실행
* `HistoryView.onRemove` 메소드 Create
  * `this.emit('@remove', { keyword })` 메소드 실행

`MainController.js` 모듈 Update

* `fetchSearchHistory` 메소드 Update
  * `HistoryView`를 `render`한 이후 메소드 체이닝으로 `bindRemoveBtn()` 메소드 실행
* `init` 메소드 Update
  * `HistoryView`를 `setup`하는 부분에서 `'@remove'` 이벤트를 `on` 메소드로 등록
    * 이벤트 리스너로 `e => this.onRemoveHistory(e.detail.keyword)` 등록
* `onRemoveHistory` 메소드 Create
  * `HistoryModel`의 `remove` 메소드로 해당 `keyword`에 해당하는 데이터 삭제
  * `this.render()` 메소드 실행하여 화면을 다시 한 번 랜더링

### 19. 1-vanilla/HistoryView4

`MainController.js` 모듈 Update

* `onChangeTab` 메소드 Update
  * 클릭한 탭의 이름을 `this.selectedTab` 에 할당
  * `this.renderView()` 메소드 실행
* `init` 메소드 Update
  * 초기 `this.selectedTab` 값을 다시 `'추천 검색어'` 로 변경

### 20. 1-vanilla/HistoryView5

`MainController.js` 모듈 Update

* `search` 메소드 Update
  * 추천 검색어 클릭, 최근 검색어 클릭, 직접 입력 모두 최종적으로 `search` 메소드를 호출하기 때문
  * `HistoryModel.add(query)` 메소드 실행
    * `HistoryModel` 에 검색 기록을 추가하는 메소드


## 3. Vue.JS

해당 브랜치의 주제를 정리했습니다.

1.  [scafolding](#1-2-vue/scafolding)
2.  [install](#2-2-vue/install)
3.  [Form1](#3-2-vue/form1)
4.  [Form2](#4-2-vue/from2)
5.  [Result1](#5-2-vue/result1)
6.  [Result2](#6-2-vue/result2)
7.  [Tab1](#7-2-vue/tab1)
8.  [Tab2](#8-2-vue/tab2)
9.  [Keyword](#9-2-vue/keyword)
10. [History1](#10-2-vue/history1)
11. [History2](#11-2-vue/history2)

### 1. 2-vue/scafolding

Vue.js 를 이용해 MVVM 패턴의 웹 애플리케이션을 만들기 위한 기본 폴더 구조

### 2. 2-vue/install

`index.html` 파일 Update

* Vue.js 를 CDN 방식을 이용해 설치
  * `app.js` 모듈을 읽어오는 `script` 태그 바로 위에 Vue.js 를 읽어오는 `script` 태그 작성
* `body` 태그 아래의 최상단 `div` 태그에 `#app` 으로 `id` 값 설정
  * Vue Instance 가 해당 `div` 태그 (DOM) 에 마운팅
  * `div.container` 내부에 `{{ msg }}` 작성
    * Vue Instance 의 `data` 중에 `msg` 를 출력

`app.js` 모듈 Update

* 새로운 Vue Instance 생성
  * `new Vue({ ... })`
    * `el` 속성으로는 `'#app'` 지정
    * `data` 속성으로 객체 지정
      * `msg` 속성에 `'hello world'` 값 할당

### 3. 2-vue/Form1

`index.html` 파일 Update

* `form` 태그 작성
  * 1-vanilla/index.html 의 `form` 태그 영역을 그대로 복사
* `input` 태그에 Vue Instance 의 `query` 데이터 바인딩
  * `v-model="query"`
* `button` 태그가 Vue Instance 의 `query` 데이터의 길이에 따라 나타나도록 설정
  * `v-show="query.length"`
* `form` 태그에 `submit` 이벤트에 대한 이벤트 리스너 작성
  * `v-on:submit.prevent="onSubmit"`
  * `.prevent` 는 HTML 기본 이벤트를 막아줌
    * 화면이 자동으로 갱신되는 것을 막기 위함

`app.js` 모듈 Update

* `query` 데이터 생성
  * 빈 문자열
  * 사용자가 입력한 값과 바인딩
    * `input` 태그에 `v-model` 로 바인딩
* `methods` 항목 작성
  * `onSubmit` 메소드 작성

### 4. 2-vue/From2

`index.html` 파일 Update

* `form>button` 태그에 `click` 이벤트 리스너 등록
  * `v-on:click="onReset"`
* `form/input` 태그에 `keyup` 이벤트 리스너 등록
  * `v-on:keyup="onKeyup"`

`app.js` 모듈 Update

* `onReset` 메소드 Create
  * `this.query = ''`
    * 해당 Vue Instance 의 `query` 데이터를 빈 문자열로 바꿈
* `onKeyup` 메소드 Create
  * 만일 `query` 의 길이가 없다면 `onReset()` 메소드 호출
  * `if (!this.query.length) this.onReset()`

### 5. 2-vue/Result1

`app.js` 모듈 업데이트

* `SearchModel` 모듈 `import`
* 검색 결과를 나타내는 `searchResult` 데이터 Create
  * 빈 배열의 형태
* `onSubmit` 메소드 Update
  * `this.search()` 메소드 실행
* `search` 메소드 Create
  * `SearchModel.list()` 메소드를 실행하여 검색 결과 데이터 조회
  * `.then()` 메소드 체이닝으로 조회한 데이터 처리
    * `this.searchResult` 데이터에 조회한 데이터 할당
* `submitted` 데이터 Create
  * 초기값은 `false`
  * 검색이 일어나면 (`search` 메소드가 실행되면) `true` 로 값 변경

`index.html` 모듈 Update

* 검색 결과를 출력하는 영역을 `div` 태그로 감쌈
  * `v-if="submitted"` 디렉티브로 Vue Instance 의 `submitted` 데이터가 `true` 일 때만 랜더링하도록 함

### 6. 2-vue/Result2 

`app.js` 모듈 Update

* `resetForm` 메소드 Update
  * `this.submitted = false`
    * 검색을 시도했는지 나타내는 데이터를 다시 `false` 로 바꿈
  * `this.searchResult = []`
    * 검색 결과를 담고 있는 배열을 다시 빈 배열로 바꿈

### 7. 2-vue/Tab1

`index.html` 모듈 Update

* `div[v-if="submitted"]` 태그 아래에 `div[v-else]` 태그 작성
  * Vue Instance 의 `submitted` 데이터가 `false` 일 때 출력
  * `ul[class="tabs"]` 태그 작성
    * `li[v-for="tab in tabs"][v-bind:class="{active: tab === selectedTab}"]` 태그 작성
      * `v-for` 디렉티브로 반복 랜더링
      * `{{ tab }}` 으로 `tab` 내용 출력
      * `tab` 과 Vue Instance 의 `selectedTab` 데이터가 동일한 경우 `class` 로 `active` 부여

`app.js` 모듈 Update

* `tabs` 데이터 Create
  * `['추천 검색어', '최근 검색어']`
* `created` 라이프 사이클 메소드 Create
  * `this.selectedTab = this.tabs[0]`
  * `selectedTab` 데이터를 `tabs` 배열의 첫 번째 인자로 초기화

### 8. 2-vue/Tab2

`index.html` 모듈 Update

* 탭을 나타내는 `li` 태그에 `v-on:click="onClickTab(tab)"` 디렉티브 추가
  * 클릭 이벤트에서 `onClickTab` 메소드에 `tab` 을 첫 번째 인자로 전달하여 메소드 실행
* `div[v-if="selectedTab === tabs[0]"]` 태그 작성
  * 추천 검색어 목록을 위한 태그
* `div[v-else]` 태그 작성
  * 최근 검색어 목록을 위한 태그

`app.js` 모듈 Update

* `selectedTab` 데이터에 빈 문자열 할당하여 Create
  * 초기에 선언해 놓지 않으면 메소드에서 접근할 수 없기 때문
* `onClickTab` 메소드 Create
  * `tab` 을 첫 번째 인자로 받음
  * `this.selectedTab = tab` 으로 현재 선택한 탭 변경

### 9. 2-vue/Keyword

`app.js` 모듈 Update

* `KeywordModel` import
* `keywords` 데이터 Create
  * 빈 배열 할당
* `created` 라이프 사이클 메소드 Update
  * `this.fetchKeyword()` 메소드 실행
* `fetchKeyword` 메소드 Create
  * `KeywordModel.list().then(data => this.keywords = data)` 실행
* `onClickKeyword` 메소드 Create
  * `this.query = keyword`
    * 검색어를 키워드로 설정
  * `this.search()` 메소드 실행
    * 검색 실행

`index.html` 모듈 Update

* 추천 검색어 목록 출력하는 영역에 `div[v-if="keywords.length"]` 태그와 `div[v-else]` 태그 작성
  * `div[v-if="keywords.length"]`
    * `ul[class="list"]` 태그 작성
      * `li[v-for="(item, index) in keywords"][v-on:click="onClickKeyword(item.keyword)"]` 태그 작성
        * `span[class="number"]{ {{ index+1 }} }` 로 추천 검색어 목록 번호 출력
        * {{ item.keyword }} 로 추천 검색어 출력
  * `div[v-else]`
    * `'추천 검색어가 없습니다.'` 출력

### 10. 2-vue/History1

`index.html` 모듈 Update

* 최근 검색어 목록 출력하는 영역에 `div[v-if="history.length"]` 태그와 `div[v-else]` 태그 작성
  * `div[v-if="history.length"]`
    * `ul[class="list"]` 태그 작성
      * `li[v-for="item in history"][v-on:click="onClickKeyword(item.keyword)"]` 태그 작성
        * 추천 검색어에서 사용한 `onClickKeyword` 메소드 그대로 사용
        * 같은 일을 수행하기 때문
        * `{{ item.keyword }}` 로 최근 검색어 출력
        * `span[class="date"]{ {{item.date}} }` 로 검색 날짜 출력
        * `button[class="btn-remove"]` 로 최근 검색어 삭제 버튼 출력
  * `div[v-else]`
    * `'최근 검색어가 없습니다.'` 출력

`app.js` 모듈 Update

* `HistoryModel` 모듈 import
* `history` 데이터 Create
  * 초기값으로 빈 배열 할당
* `created` 라이프 사이클 메소드 Update
  * `this.fetchHistory()` 메소드 실행
* `fetchHistory` 메소드 Create
  * `HistoryModel.list().then(data => this.history = data)`
    * 최근 검색어 목록을 조회해서 `history` 데이터에 할당

### 11. 2-vue/History2

`index.html` 모듈 Update

* 최근 검색어의 삭제 버튼에 `v-on:click.stop="onClickRemoveHistory(item.keyword)"` 이벤트 리스너 작성

`app.js` 모듈 Update

* `onClickRemoveHistory(keyword)` 메소드 Create
  * `HistoryModel.remove(keyword)`
  * `this.fetchHistory()`
* `search` 메소드 Update
  * `HistoryModel.add(this.query)`
  * `this.fetchHistory()`

## 4. Component

해당 브랜치의 주제를 정리했습니다.

1. [scafolding](#1-3-component/scafolding)
2. [FormComponent1](#2-3-component/formcomponent1)
3. [FormComponent2](#3-3-component/formcomponent2)
4. [ResultComponent](#4-3-component/resultcomponent)
5. [ListComponent1](#5-3-component/listcomponent1)
6. [ListComponent2](#6-3-component/listcomponent2)
7. [TabComponent1](#7-3-component/tabcomponent1)

### 1. 3-component/scafolding

2-vue 브랜치에서 마지막에 작업한 결과 그대로 가져옴
Vue Component를 사용하기 위한 준비 단계

### 2. 3-component/FormComponent1

`index.html` 모듈 Update

* `form` 태그 영역을 HTML 문서 하단에 `template#search-form` 태그 안으로 이동
  * `FormComponent` 에서 `template` 속성으로 연결할 태그
* 등록한 `search-form` 디렉티브로 `FormComponent` 사용
  
`app.js` 모듈 Update

* `FormComponent.js` 모듈 import
* Vue Instance 의 `components` 항목에 컴포넌트 등록
  * `{ 'search-form': FormComponent }`

`FormComponent.js` 모듈 Create

* `export default { ... }` 로 객체를 `export`
  * 해당 객체가 Vue Component
  * `template` 으로 `#search-form` 지정
  * `data`에 `query` 생성
    * 빈 문자열로 초기화
  * `methods` 에 `onSubmit`, `onKeyup`, `onReset` 메소드 정의

### 3. 3-component/FormComponent2

`FormComponent.js` 모듈 Update

* `props` 항목에 `['value']` 등록
* `data` 항목의 `query` 데이터를 `inputValue` 로 변경하고 초기값으로 `this.value` 할당
* `onSubmit` 메소드 Update
  * `this.$emit('@submit', this.inputValue.trim())` 으로 `'@submit'` 이라는 이름의 이벤트 발생하고 입력값을 함께 전달
* `onReset` 메소드  Update
  * `this.inputValue = ''` 로 입력값 초기화
  * `this.$emit('@reset')` 으로 `'@reset'` 이라는 이벤트 발생
* `onKeyup` 메소드 Update
  * 입력값이 없는 경우 `this.onReset()` 메소드 실행

`index.html` 모듈 Update

* `search-form` 컴포넌트 디렉티브에 `v-bind:value="query"` 디렉티브 사용
  * `app.js` 의 `query` 데이터를 `FormComponent` 내부의 `value` 값으로 주입
* `search-form` 컴포넌트 디렉티브에 `v-on:@submit="onSubmit"` 디렉티브 사용
  * `FormComponent` 내부에서 `'@submit'` 이라는 이벤트가 발생하면 `app.js` 의 `onSubmit` 메소드가 처리
* `search-form` 컴포넌트 디렉티브에 `v-on:@reset="onReset"` 디렉티브 사용
  * `FormComponent` 내부에서 `'@reset'` 이라는 이벤트가 발생하면 `app.js` 의 `onReset` 메소드가 처리


`app.js` 모듈 Update

* `onSubmit` 메소드 Update
  * 받는 인자의 이름을 `query` 로 변경
  * `this.query` 에 인자로 받은 `query` 값 할당
  * 그 이후에 이전과 동일하게 `this.search()` 메소드 실행
* `onKeyup` 메소드 Delete
  * `FormComponent.js` 모듈 안으로 완전히 이동

### 4. 3-component/ResultComponent

`ResultComponent.js` 모듈 Create

* `template` 에 `'#search-result'` 등록
* `props` 에 `['data', 'query']` 등록

`index.html` 모듈 Update

* 검색 결과를 나타내는 영역을 `template#search-result` 태그 안 쪽으로 이동
  * `searchResult` 를 `data` 로 변경
* 검색 결과를 나타내는 영역에는 `<search-result</search-result>>` 컴포넌트 디렉티브 사용
  * `v-bind:data="searchResult"` 디렉티브로 `app.js` 의 `searchResult` 데이터를 `ResultComponent` 에 `data` 라는 이름의 `prop` 으로 전달
  * `v-bind:query="query"` 디렉티브로 `app.js` 의 `query` 데이터를 `ResultComponent` 에 `query` 라는 이름의 `prop` 으로 전달

`app.js` 모듈 Update

* `ResultComponent` 모듈 `import`
* `components` 에 `ResultComponent` 를 `'search-result'` 라는 이름으로 등록

### 5. 3-component/ListComponent1

`ListComponent.js` 모듈 Create

* `template` 에 `#list` 등록
* `props` 에 `['data', 'type']` 등록
* `methods` 에 `onClickList`, `onRemoveList` 메소드 정의
  * `onClickList` 메소드에서는 `this.$emit('@click', keyword)`
  * `onRemoveList` 메소드에서는 `this.$emit('@remove', keyword)`

`index.html` 모듈 Update

* `template#list` 태그 생성
  * 추천 검색어 목록과 최근 검색어 목록의 템플릿을 모두 취합하여 `template#list` 태그 안에 작성
  * 데이터나 메소드 이름을 일반적인 형태로 변경
  * `type` `prop` 에 따라 목록에서 선택적으로 랜더링
    * 번호는 추천 검색어 목록에서만 출력
    * 날짜와 삭제 버튼은 최근 검색어 목록에서만 출력
* 추천 검색어 목록이 있었던 곳은 `list[v-bind:data="keywords"][type="keywords"]` 컴포넌트 디렉티브로 대체
  * `v-on:@click="onClickKeyword"` 로 이벤트 바인딩
* 최근 검색어 목록이 있었던 곳은 `list[v-bind:data="history"][type="history"]` 컴포넌트 디렉티브로 대체
  * `v-on:@click="onClickKeyword"` 로 이벤트 바인딩
  * `v-on:@remove="onClickRemoveHistory"` 로 이벤트 바인딩

`app.js` 모듈 Update

* `ListComponent.js` 모듈 `import`
* `components` 에 `ListComponent` 를 `'list'` 라는 이름으로 등록

### 6. 3-component/ListComponent2

`ListComponent.js` 모듈 Update

* `computed` 로 `keywordType`, `historyType` 등록
  * 각각 `this.type` 이 `'keywords'` 인지 `'history'` 인지 판단하는 `computed` 속성

`index.html` 모듈 Update

* `v-if` 디렉티브에서 `type` 을 비교하고 있던 부분을 `keywordType`, `historyType` 으로 변경

`FormComponent.js` 모듈 Update

* `watch` 에 `value` 등록
  * 새 `value` `prop` 이 들어오면 `this.inputValue` 를 새로운 `newVal` 값으로 업데이트

### 7. 3-component/TabComponent1

`index.html` 모듈 Update

* `template#tabs` 태그 작성
* 기존 탭 영역을 주석처리
* 탭 영역 자리에 `<tabs></tabs>` 컴포넌트 디렉티브 작성

`TabComponent.js` 모듈 Create

* `template` 에 `'#tabs'` 등록

`app.js` 모듈 Update

* `TabComponent` 모듈 `import`
* `components` 에 `TabComponent` 를 `'tabs'` 라는 이름으로 등록
