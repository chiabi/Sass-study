<<<<<<< HEAD
## Sass Chapter3

- Chorme V8 엔진 기반의 플랫폼 구성 : Node.js & NPM 
- Node.js 기반 프론트-엔드 개발 작업 자동화 빌드 시스템 : Gulp.js

### 1. [Node](https://nodejs.org/ko/)
 - 자바스크립트를 서버사이드 언어로 사용할 수 있다.
 - 자바스크립트 언어로 사용자 시스템 환경 정보에 접근하거나 조작할 수 있다.
 - [npm](https://www.npmjs.com/) : 노트 패키지 매니저

### 2. [Gulp](http://gulpjs.com/)
 - Gulp를 전역적으로 설치하기
```
$ npm install --global gulp-cli
$ gulp -v : 버전확인
```

 - 개별적인 프로젝트에 Gulp 로컬 설치 
 	: 인터넷이 지원되지 않는 상황에서 gulp 설치가 필요할 수 있기 때문
```
$ npm i --save-dev gulp : 개발할 때만 의존하는 모듈로 package.json이 기술됨, -D로 줄여쓸 수 있음
('--save' 명령어 입력시 배포할 때도 의존하는 모듈로 기술됨, -S로 줄여쓸 수 있음 )
``` 

 - gulp-sass, gulp-compass(gulp-sass + compass), gulp-ruby-sass

 - gulp-sass-compass.zip활용
	* 압축을 풀고 $ npm install로 설치
 	* 정상 설치 시 파일에 node_modules와 하부 파일이 생성됨
 		- browser-sync(코드 변경 시 브라우저 자동으로 새로고침), gulp, gulp-compass, gulp-if, gulp-minify-html, gulp-util
 	* $ gulp-compass로 실행
 	* config.js등 설정 파일에서의 변경은 gulp를 재실행해야 반영됨
 	* 작업은 src에서 build는 최종 파일
=======
## Sass Study 자료 

- **[Sass Chapter1](../../tree/master/chapter1)** : 실습 환경설정, Sass설치, Git Bash, Snippet
- **[Sass Chapter2](../../tree/master/chapter2)** : Sass 가이드 라인
- **[Sass Chapter3](../../tree/master/chapter3)** : Node, Gulp
>>>>>>> a2ca45b4ae2fee6db38c7baf1db6504ecf5881d2
