## Sass 

### 1. Sass 실습 환경설정

- 에디터 : **[Sublime Text 3](https://www.sublimetext.com/3)**
	* [Package Control](https://packagecontrol.io/)
	* [Emmet](http://docs.emmet.io), [Emmet 스니펫/축약코드](http://docs.emmet.io/cheat-sheet/)
	* SideBarEnhancements, Syntax Highlighting for Sass, Color Picker, IMESupport, ConvertToUTF8

- 버전관리 도구 : **[Git / GitHub / Git Bash](https://git-scm.com/)**
	* [Octotree](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc)

- 플랫폼 : Sass, Node
	* **[Ruby](https://www.ruby-lang.org/ko/)**, [Ruby Download for Windows](http://rubyinstaller.org/)
	* **[Node](https://githubhttps://nodejs.org/en/)**

- 플랫폼 별 Sass
	* **[Ruby Sass](http://sass-lang.com/)**
	* **[Node Sass](https://github.com/sass/node-sass)**

-

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

-

### 3. Git Bash 명령어

```sh
	- cd directory-name : 디렉토리 이동
	- cd ~ : Git Bash를 처음 실행했을 때의 위치로
	- cd ..(/..) 상위 디렉터리로 이동
	- mkdir directories-name : 생성할 디렉토리 이름 나열
	- touch directories-name/files-name : 생성할 파일 이름 나열
	- ls : 디렉터리 안 파일 목록 출력
	- ls -l : 파일목록과 상세정보 출력
	- mv directory-name/file-name directory-name/file-name : 파일 위치 이동 또는 이름 변경
	- pwd : 현재 디렉터리의 정학한 경로 확인
	- vim file-name : vim 에디터 실행 (문서작성 완료 시 [esc] > ":wq"입력)
	- cat file-name : 파일 내용을 화면에 출력
	- cp directory-name/file-name directory-name/file-name : 파일 및 디렉터리 복제 
	- cp -R directory-name/ directory-name/ : 디텍터리 통째로 복제
	- rm file-name : 파일 삭제
	- rmdir directory-name : 빈 디렉터리 삭제
	- rm -rf directory-name : 비어있지 않은 디렉터리 강제로 삭제
```

#### Git Bash 한글 깨짐 문제 / .bashrc파일과 [alias](https://git-scm.com/book/ko/v2/Git%EC%9D%98-%EA%B8%B0%EC%B4%88-Git-Alias)

```sh
alias ls="ls -ph --show-control-chars"
alias ls="lsa -al --show-control-chars"

alias swet="sass -w -E -utf-8 -t"

alias gs="git status"
alias gc="git commit"
alias ga="git add"
alias gcam="git commit -a -m"
alias glog="git log"
```