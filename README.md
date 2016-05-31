## Sass 

### 1. Sass 실습 환경설정

- 에디터 : **[Sublime Text 3](https://www.sublimetext.com/3)**
	* [Package Control](https://packagecontrol.io/)
	* Emmet, SideBarEnhancements, Syntax Highlighting for Sass, Color Picker, IMESupport, ConvertToUTF8

- 버전관리 도구 : **[Git / GitHub / Git Bash](https://git-scm.com/)**
	* [Octotree](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc)

- 플랫폼 : Sass, Node
	* **[Ruby Sass](http://sass-lang.com/)**, [Ruby Download for Windows](http://rubyinstaller.org/)
	* **[Node Sass](https://github.com/sass/node-sass)**

-----------------------------------------

### 2. Sass 설치

#### **[rubygems](https://rubygems.org/gems/sass)**

```sh
	- REQUIRED RUBY VERSION : 최소 지원되는 루비 버전
	- 설치 : gem install sass
	- 설치 확인 : gem list sass
	- gem 설치 된 모든 파일 확인 : gem list *
	- 설치된 구버전 sass 삭제 : gem uninstall sass > (버전 선택)
```

#### Ruby Gem 설치 오류 발생시 

- *윈도에서 오류 생길 경우 gem을 끌어오는 기본주소가 안될 경우 지우고 다른 주소로 add함

```sh
$ gem source --add https://s3.amazonaws.com/production.s3.rubygems.org/
$ gem source --remove https://rubygems.org/
```