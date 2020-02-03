# chap01. npm & create-react-app

## npm을 이용해서 create react app 설치
```
# 터미널창에서 다음 명령어를 실행합니다. (g는 글로벌 , 컴퓨터 어디서든 앱을 실행하는 옵션.)
npm install -g create-react-app   
```

## create-react-app 생성 & 실행
```
# 프로젝트를 생성하고자 하는 폴더로 이동합니다.
cd react-app

# create-react-app 명령을 통해 프로젝트를 생성합니다. (.은 현재디렉토리)
create-react-app . 

# 다음 명령어로 앱을 실행합니다.
npm run start
```


# chap02. 컴포넌트 만들기
## chap02_1. 리액트가 없을때의 상황
```
create-react-app에서 public폴더는 npm run start를 실행했을때 파일을 찾는 document root 이다.
pure.html 들어있는 내용은 작지만 실제로 많은 코드가 들어갈 경우 한눈에 파악하기란 쉽지않다.
header태그 , nav태그 , article태그의 내용을 각각 분리하여 따로 관리할수 있다면??!
```

## chap02_2. 컴포넌트 만들기 1
```
App.js에 Subject라는 이름의 컴포넌트 만든다.
컴포넌트를 만들때 주의할 점은 랜더링 내용을 반드시 최상위 태그로 이루어져야한다.
localhost:3000/pure.html와 localhost:3000을 비교하여 결과확인.
App.js를 보면 랜더링할 내용에 태그를 따옴표 없이 그대로 html 문법처렁 사용하는데 이것은 페이스북에서 만든 jsx문법이다. 더 쉽게 빠르게하기 위해 만들었으며 jsx가 자동으로 웹브라우져에서 실행될 수 있도록 자바스크립트 문법으로 컨버팅 해준다.
```