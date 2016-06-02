## Sass Chapter2

### 1. Sass 가이드 라인

- [Sass Documentation](http://sass-lang.com/documentation/file.SASS_REFERENCE.html)
- [Sass Guideline](https://sass-guidelin.es/ko/)

---

#### 프로젝트 트리 구조(Project Tree Structure)
```sh
	*
	|
	├─ READEME.md
	├─ index.html
	├─ js/
	| 	└─ vender/
	| 		└─ modernizr.js
	├─ sass/
	|	├─ style.sass
	|	├─ modules/ 
	|	|	├─ common/ 
	|	|	|	└─ _common.sass	
	|	|	├─ grid-system/
	|	|	|	└─ _grid.sass		
	|	|	├─ init/			
	|	|	|	├─ _normalize.scss
	|	|	|	└─ _reset.scss
	|	|	└─ rwd/
	|	|		└─ _rwd.sass
	|	└─ pages/
	|		└─ _skip-to-content.sass
	|
	└─ css/
		└─ style.css
```