README
=============================================================================================================
* `history.replaceState()`는 IE 10부터 지원.
  >https://caniuse.com/#search=replacestate
* IE에서도 브라우저의 history를 다룰 수 있는 오픈소스를 fork하였음.
* 사용법은 해당 GitHub 참고.
>https://github.com/devote/HTML5-History-API

### 추가된 파일
#### history.ielte7_custom.js
* 오픈소스 원본에서 수정한 버전.
* IE에서 replaceState 사용시 기존 URL 뒤에 '#'이 붙으면서 append되는 부분 수정.
#### custom_history.js
* `history.ielte7_custom.js`를 외부에서 객체로 사용할 수 있게 수정한 버전.
* 오픈소스를 이용했지만, `window.history`에 property가 override 되어서 오픈소스 수정하여 override 되지 않고 동작시키는 방법 생각해야 함.
* IE 7 이하에서는 오픈소스 내에서 "addEventListener" 이벤트를 덮어씌우는 동작이 있어 광고주 홈페이지와 충돌하여 JS 오류 발생.
