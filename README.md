# EDIYA (Sass 버전)

**[이듬(E.UID)](https://euid.dev) 블렌디드 러닝, 학습용(디자인 → 개발)** 으로 제작된 Sass 버전의 [이디야 커피 브랜드 사이트](https://seulbinim.github.io/EDIYA-Sass/)입니다.

## Sass 및 PostCSS 환경구성

**EDIYA-Sass 폴더 복제하기**
```
git clone https://github.com/seulbinim/EDIYA-Sass.git
```

**.git 디렉토리 삭제**
```
cd EDIYA-Sass
rm -rf .git
```

**개발의존성 모듈 설치**
```
npm install
```

## npm 명령어

```
npm run 명령어
```
> start 명령의 경우 run을 생략할 수 있다.  

| 명령어 | 설명 |
|-|-|
| start | dev 명령과 watch:htmlhint 및 watch:sass 명령을 병렬로 수행 |
| htmlhint | 현재 프로젝트에 포함 된 모든 html 파일에 대해 HTML Validation을 수행 |
| watch:htmlhint | 파일 내용이 변경되었을 때 HTML Validation을 수행 |
| sass | sass 파일을 css 파일로 빌드 |
| watch:sass | 파일 내용이 변경되었을 때 sass 파일을 css 파일로 빌드 |
| build:postcss | postcss 플러그인을 사용하여 css 파일을 재 빌드 |
| build | build:sass 명령과 build:postcss 명령을 직렬로 수행 |

**참고 사이트**  
- [htmlhint](https://www.npmjs.com/package/htmlhint) 
- [html watch](https://github.com/htmlhint/HTMLHint/issues/135#issuecomment-267123306)
- [sass](https://www.npmjs.com/package/sass)
- [postcss-cli](https://github.com/postcss/postcss-cli)
- [postcss plugins](https://github.com/postcss/postcss/blob/main/docs/plugins.md)
- [postcss-autoprefixer](https://github.com/postcss/autoprefixer)
- [postcss-csso](https://github.com/lahmatiy/postcss-csso)
- [postcss-combine-media-query](https://github.com/SassNinja/postcss-combine-media-query)