# 인프런 '실습 UI 개발로 배워보는 순수 JS와 VueJS 개발' 강좌 따라하기
> 강좌에서 제공하는 github repo 를 fork 해서 정리한 내용입니다.

## 둘러보기

0. [들어가며](#0-들어가며)
1. [브랜치 순서](#1-브랜치-순서)
2. [VanillaJS](#2-vanillajs)

## 0. 들어가며

인프런의 '실습 UI 개발로 배워보는 순수 JS와 VueJS 개발' 강좌를 들으면서 실습을 진행한 내용입니다.

강좌에서 제공한는 repo 를 fork 해서 실습한 내용을 추가했습니다.

## 1. 브랜치 순서

강좌 진생 순서별로 어떤 브랜치를 찾아가야 하는지 정리한 내용입니다.

1. Lecture 5 - 순수JS (MVC)/폴더 구조 : 1-vanilla/scafolding
2. Lecture 6 - 검색폼/검색폼 구현 1 : 1-vanilla/controller
3. Lecture 7 - 검색폼/검색폼 구현 2 : 1-vanilla/FormView1
4. Lecture 8 - 검색폼/검색폼 구현 3 : 1-vanilla/FormView2
5. Lecture 9 - 검색폼/검색폼 구현 4 (실습) : 1-vanilla/FormView3

## 2. VanillaJS

해당 브랜치의 주제를 정리했습니다.

1. [scafolding](#1-scafolding)
2. [controller](#2-controller)
3. [FormView1](#3-formview1)
4. [FormView2](#4-formview2)
5. [FormView3](#5-formview3)
6. [FormView4](#6-fromview4)

### 1. scafolding

vanillaJS 로 MVC 패턴을 구현할 때 사용하는 폴더 구조

### 2. controller

`MainController.js` 모듈 작성 및 등록
- `console.log()` 로 정상 작동하는지 출력

크롬 61 버전 이상부터 ES6 의 module system 지원

### 3. FormView1

`FormView.js` 모듈 작성  
- `View.js` 모듈을 상속 받아 작성
- `FormView.setup` 메소드 작성
  - 인자로 받은 form 엘리먼트 (`el`) 를 프로퍼티에 등록
  - form 엘리먼트 (`el`) 의 text input 엘리먼트 (`el.querySelector('[type=text]')`) 를 `inputEl` 프로퍼티에 등록
  - form 엘리먼트 (`el`) 의 reset button 엘리먼트 (`el.querySelector('[type=reset]')`) 를 `resetEl` 프로퍼티에 등록
  - `FormView.showResetBtn()` 메소드를 `false` 인자를 전달하면서 실행
- `FormView.showResetBtn` 메소드 작성
  - 인자 `show` 로 `Boolean` 값 받음, 기본값은 `true`
  - 등록되어 있는 `resetEl` 의 `style.display` 프로퍼티 (`this.resetEl.style.display`) 값을 변경
    - `show` 인자가 `true` 라면 `'block'`
    - `show` 인자가 `false` 라면 `'none'`

`FormView.js` 모듈을 `MainController.js` 모듈에 등록
- `MainController.js` 의 `init()` 메소드에서 `FormView.setup()` 메소드 실행
  - 인자로는 form 엘리먼트 (`document.querySelector('form')`) 전달

실행 결과 첫 로딩 화면에서 reset button 은 화면에 표시되지 않음

### 4. FormView2

`FormView.js` 모듈 업데이트
- `FormView.setup()` 메소드에서 `this.bindEvents()` 메소드 호출
- `FormView.bindEvents` 메소드 작성
  - `this` (form 엘리먼트) 에 `'submit'` 이벤트 리스터 작성 (`View.js` 모듈에서 상속받은 `this.on()` 메소드 사용)
    - `e.preventDefault()` 로 form 엘리먼트의 기본 이벤트 방지
    - 엔터키를 누르면 폼 전송을 위해 화면 갱신이 이루어지는 기본 이벤트
  - 등록되어 있는 `this.inputEl` 엘리먼트에 `keyup` 이벤트 리스너 작성 (기본 `addEventListener()` 메소드 사용)
    - `this.onKeyup()` 메소드 실행 (인자로 이벤트 객체 넘겨줌)
- `FormView.onKeyup` 메소드 작성
  - `this.showResetBtn()` 메소드 실행
    - 인자로 `this.inputEl.value.length` 전달
      - `value` 값이 없다면 `length` 가 `0` 이므로 `false`
      - `value` 값이 있다면 `length` 가 자연수이므로 `true`

### 5. FormView3

`FormView.js` 모듈의 `FormView.onKeyup` 메소드 업데이트
- 엔터 키 코드 (`13`) 를 `enter` 상수에 정의
- 입력한 키가 엔터 키인지 확인
  - 엔터 키가 아니면 `return` 으로 함수 종료
  - 엔터 키라면 `this.emit()` 메소드 실행 (`View.js` 모듈에서 상속받음)
    - `'@submit'` 이라는 커스텀 이벤트 발생시킴
    - `{ input: this.inputEl.value }` 객체를 `emit` 메소드의 두 번째 인자 (`data`) 로 전달

`MainController.js` 모듈 업데이트
- `init` 메소드에서 `FormView.setup()` 메소드를 호출한 후 메소드 체이닝으로 `on()` 메소드 실행
  - `FormView.setup` 메소드, `FormView.on` 메소드에서 `this` (`FormView` 객체 자신) 를 `return` 하기 때문에 가능
  - `on` 메소드는 `View.js` 모듈에게 상속받은 것
  - `'@submit'` 이벤트에 대한 리스너 작성
    - `MainController.js` 모듈 (화살표 함수에서 `this` 는 외부 함수의 맥락을 따름, 본래 `addEventListener` 의 callback 함수 안에서 `this` 는 이벤트가 발생한 DOM 엘리먼트임) 의 `this.onSubmit()` 메소드 실행
      - 인자로 `e.detail.input` 값 전달 (`FormView.js` 모듈의 `FormView.onKeyup` 메소드 내부에서 `'@submit'` 이벤트를 발생시킬 때 전달한 객체)
- `onSubmit` 메소드 작성
  - `console.log()` 로 결과 출력해서 확인

### 6. FormView4

`FormView.js` 모듈 업데이트
- `FormView.bindEvents` 메소드 업데이트
	- 등록되어 있는 `this.resetEl` 엘리먼트에 `click` 이벤트 리스너 작성 (기본 `addEventListener()` 메소드 사용)
		- `this.onClickReset()` 메소드 실행
- `FormView.onClickReset` 메소드 작성
  - `this.emit()` 메소드 실행 (`View.js` 모듈에서 상속받음)
    - 인자로 `'@reset'` 전달 (`'@reset'` 이벤트 발생시킴)
	- `this.showResetBtn(false)` 메소드 실행
		- 리셋 버튼 안 보이게 함
- `FormView.onKeyup` 메소드 업데이트
	- `this.inputEl.value.length` 값이 존재하지 않는다면 (`0` 이라면) `this.emit('@reset')` 메소드 실행

`MainController.js` 모듈 업데이트
- `init` 메소드 업데이트
	- `FormView.setup().on()` 메소드 체이닝에 `FormView.on()` 메소드 추가
		- `'@reset'` 이벤트 감지
		- `this.onResetForm()` 메소드 실행
- `onResetForm` 메소드 작성
	- `console.log()` 로 결과 출력해서 확인

현재 reset 버튼은 `input[type=reset]` 이기 때문에 기본으로 클릭하면 `input[type=text]` 의 내용 삭제함