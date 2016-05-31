## Sass Chapter1

### 1. Sass 실습 환경설정

- 에디터 : **[Sublime Text 3](https://www.sublimetext.com/3)**
	* [Package Control](https://packagecontrol.io/)
	* [Emmet](http://docs.emmet.io), [Emmet 스니펫/축약코드](http://docs.emmet.io/cheat-sheet/)
	* SideBarEnhancements, Syntax Highlighting for Sass, Color Picker, IMESupport, ConvertToUTF8
	* [win chear sheet(영문)](https://www.shortcutfoo.com/app/dojos/sublime-text-3-win/cheatsheet)

- 버전관리 도구 : **[Git / GitHub / Git Bash](https://git-scm.com/)**
	* [Octotree](https://chrome.google.com/webstore/detail/octotree/bkhaagjahfmjljalopjnoealnfndnagc)

- 플랫폼 : Sass, Node
	* **[Ruby](https://www.ruby-lang.org/ko/)**, [Ruby Download for Windows](http://rubyinstaller.org/)
	* **[Node](https://githubhttps://nodejs.org/en/)**

- 플랫폼 별 Sass
	* **[Ruby Sass](http://sass-lang.com/)**
	* **[Node Sass](https://github.com/sass/node-sass)**

---

### 2. Sass 설치

#### **[rubygems](https://rubygems.org/gems/sass)**

- *REQUIRED RUBY VERSION : 최소 지원되는 루비 버전
```sh
	$ gem install sass : 설치
	$ gem list sass : 설치 확인
	$ gem list * : gem 설치 된 모든 파일 확인
	$ gem uninstall sass > (버전 선택) : 설치된 구버전 sass 삭제
```

-

#### Ruby Gem 설치 오류 발생시 

- *윈도에서 오류 생길 경우 gem을 끌어오는 기본주소가 안될 경우 지우고 다른 주소로 add함

```sh
$ gem source --add https://s3.amazonaws.com/production.s3.rubygems.org/
$ gem source --remove https://rubygems.org/
```

-

#### Ruby Sass 
```sh
	$ sass --version, sass -v : 설치 된 Sass 버전 정보 확인
	$ sass --help, sass -h : Sass 명령어 도움말 정보
	$ sass [option] [input] [output]
	$ sass input.sass output.css : Sass파일을 CSS파일로 변환
	$ sass --update input.sass output.css : 업데이트
	$ sass --watch [input]:[output], sass -w : Sass폴더 내부의 파일을 CSS 폴더 내부에 변환/저장하고 관찰함 (중지: Ctrl+C)
	$ sass --style compressed, sass -t : 아웃풋 스타일
		-nested, expanded, compact, compressed
	$ sass-convert [input] [output] : Sass와 SCSS파일 간 변환
```

---

### 3. Git Bash 명령어

```sh
	$ cd directory-name : 디렉토리 이동
	$ cd ~ : Git Bash를 처음 실행했을 때의 위치로
	$ cd ..(/..) 상위 디렉터리로 이동
	$ mkdir directories-name : 생성할 디렉토리 이름 나열
	$ touch directories-name/files-name : 생성할 파일 이름 나열
	$ ls : 디렉터리 안 파일 목록 출력
	$ ls -l : 파일목록과 상세정보 출력
	$ mv directory-name/file-name directory-name/file-name : 파일 위치 이동 또는 이름 변경
	$ pwd : 현재 디렉터리의 정학한 경로 확인
	$ vim file-name : vim 에디터 실행 (문서작성 완료 시 [esc] > ":wq"입력)
	$ cat file-name : 파일 내용을 화면에 출력
	$ cp directory-name/file-name directory-name/file-name : 파일 및 디렉터리 복제 
	$ cp -R directory-name/ directory-name/ : 디텍터리 통째로 복제
	$ rm file-name : 파일 삭제
	$ rmdir directory-name : 빈 디렉터리 삭제
	$ rm -rf directory-name : 비어있지 않은 디렉터리 강제로 삭제
```

-

#### Git Bash 한글 깨짐 문제 / .bashrc파일과 **[alias](https://git-scm.com/book/ko/v2/Git%EC%9D%98-%EA%B8%B0%EC%B4%88-Git-Alias)**(별칭)

```sh
*Git Bash : 한글 깨짐 문제 (--show-control-chars)
	alias ls="ls -ph --show-control-chars"
	alias ls="lsa -al --show-control-chars"

*Sass : Windows 환경에서 한글(CP949) 오류 발생 시
	alias sass-n="sass -E UTF-8 -t nested --watch"
	alias sass-n="sass -E UTF-8 -t nested --watch"
	alias sass-c="sass -E UTF-8 -t compact --watch"
	alias sass-p="sass -E UTF-8 -t compressed --watch"

*Git 관리 명령어 Alias
	alias gs="git status"
	alias gc="git commit"
	alias ga="git add"
	alias gcam="git commit -a -m"
	alias glog="git log"
```

- Bash 설정 파일로 만들어 관리할 경우 

```sh
$ vim ~/.bashrc
	- [I]를 누름 상태바에 INSERT 가 표시되면 alias작성
``` 

---

### 4 .스니펫(Snippet)