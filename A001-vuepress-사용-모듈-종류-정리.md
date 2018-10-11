# A001-사용-모듈-종류.md

vuepress 에서 사용되고 있는 모듈의 간단한 설명 목록이다.

## 참조 

[https://github.com/vuejs/vuepress/blob/master/package.json](https://github.com/vuejs/vuepress/blob/master/package.json)

## 들어가는 글

vuepress 는 다양한 모듈을 사용하고 있다.  
각 모둘은 에반뷰가 애용하고 선택에 신중을 기한 모듈로 생각된다. 

이 모듈에 대한 사용법을 알게 되면 vuepress 를 분석하는데 도움이 되고
vue.js 패키지 사용에 도움이 될 것으로 판단된다. 

## 분석 대상 

다음 파일에 기록된 모듈 패키지들을 분석하는 것으로 시작하려고 한다. 

> vuepress/package.json

dependencies 와 devDependencies 두가지 모두 분석한다.  

## dependencies 목록

| package                            | version       |
|:-----------------------------------|:--------------|
| @babel/core                        | 7.0.0-beta.47 |
| @vue/babel-preset-app              | 3.0.0-beta.11 |
| autoprefixer                       | ^8.2.0        |
| babel-loader                       | 8.0.0-beta.3  |
| cache-loader                       | ^1.2.2        |
| chalk                              | ^2.3.2        |
| chokidar                           | ^2.0.3        |
| commander                          | ^2.15.1       |
| connect-history-api-fallback       | ^1.5.0        |
| copy-webpack-plugin                | ^4.5.1        |
| cross-spawn                        | ^6.0.5        |
| css-loader                         | ^0.28.11      |
| diacritics                         | ^1.3.0        |
| docsearch.js                       | ^2.5.2        |
| escape-html                        | ^1.0.3        |
| file-loader                        | ^1.1.11       |
| fs-extra                           | ^5.0.0        |
| globby                             | ^8.0.1        |
| gray-matter                        | ^4.0.1        |
| js-yaml                            | ^3.11.0       |
| koa-connect                        | ^2.0.1        |
| koa-mount                          | ^3.0.0        |
| koa-range                          | ^0.3.0        |
| koa-static                         | ^4.0.2        |
| loader-utils                       | ^1.1.0        |
| lodash.throttle                    | ^4.1.1        |
| lru-cache                          | ^4.1.2        |
| markdown-it                        | ^8.4.1        |
| markdown-it-anchor                 | ^5.0.2        |
| markdown-it-container              | ^2.0.0        |
| markdown-it-emoji                  | ^1.4.0        |
| markdown-it-table-of-contents      | ^0.4.0        |
| mini-css-extract-plugin            | ^0.4.1        |
| nprogress                          | ^0.2.0        |
| optimize-css-assets-webpack-plugin | ^4.0.0        |
| portfinder                         | ^1.0.13       |
| postcss-loader                     | ^2.1.5        |
| prismjs                            | ^1.13.0       |
| register-service-worker            | ^1.5.1        |
| semver                             | ^5.5.0        |
| stylus                             | ^0.54.5       |
| stylus-loader                      | ^3.0.2        |
| toml                               | ^2.3.3        |
| url-loader                         | ^1.0.1        |
| vue                                | ^2.5.16       |
| vue-loader                         | ^15.2.4       |
| vue-router                         | ^3.0.1        |
| vue-server-renderer                | ^2.5.16       |
| vue-template-compiler              | ^2.5.16       |
| vuepress-html-webpack-plugin       | ^3.2.0        |
| webpack                            | ^4.8.1        |
| webpack-chain                      | ^4.6.0        |
| webpack-merge                      | ^4.1.2        |
| webpack-serve                      | ^1.0.2        |
| webpackbar                         | ^2.6.1        |
| workbox-build                      | ^3.1.0        |

## devDependencies 목록

| package                            | version        |
|:-----------------------------------|:---------------|
| @vue/test-utils                    | ^1.0.0-beta.16 |
| babel-core                         | ^7.0.0-0       |
| babel-jest                         | ^23.0.0        |
| conventional-changelog-cli         | ^1.3.22        |
| eslint                             | ^4.19.1        |
| eslint-plugin-jest                 | ^21.15.1       |
| eslint-plugin-vue-libs             | ^3.0.0         |
| jest                               | ^23.0.0        |
| jest-serializer-vue                | ^1.0.0         |
| lint-staged                        | ^7.0.4         |
| vue-jest                           | ^2.6.0         |
| vuepress-theme-vue                 | ^1.1.0         |
| yorkie                             | ^1.0.3         |

## 패키지 설명

### autoprefixer

AutoPrefixer 플러그인은 CSS 구문을 분석해서 vendor-prefixed CSS 속성을 자동으로 추가

> https://github.com/postcss/autoprefixer

### @babel/core / babel-core

ECMAScript 6,7 으로 작성된 코드를 browser가 인식할 수 잇는 
문법(ES5)으로 변환시켜주는 transpiler

> https://github.com/babel/babel

### babel-jest

페이스북에 만든 테스트 프레임워크 Jest에서 babel 을 이용할 수 있도록 하는 플러그 인

> https://github.com/facebook/jest/tree/master/packages/babel-jest

### babel-loader

webpack에서 balbel을 이용할 수 있도록 하는 플러그 인 

> https://github.com/babel/babel-loader

### conventional-changelog-cli

깃 커밋 변경 로그를 예쁘게 정리해 주는 플러그 인 명령 처리기 

> https://github.com/conventional-changelog/conventional-changelog

### cache-loader

webpack 로더의 파일 캐쉬되도록 지원하는 플러그 인 

> https://github.com/webpack-contrib/cache-loader

### chalk

터미널 출력을 예쁘게 만들 수 있는 모듈

> https://github.com/chalk/chalk

### chokidar

파일 워치 모듈로 node.js fs.watch / fs.watchFile / fsevents 를 사용하기 쉽도록 감싼 모듈 

> https://github.com/paulmillr/chokidar

### commander

커맨드라인 입력시 사용되는 옵션을 쉽게 구현하도록 도와주는 모듈

> https://github.com/tj/commander.js/

### connect-history-api-fallback

단일 페이지 앱 SPA 을 작성할 때 새로 고침 또는 직접 url 지정으로 생기는 
없는 페이지 또는 이전 페이지 이동시 문제를 /help 또는 /help/online 같은 
페이지로 연결하거나 간단한 캐쉬 처리를 함으로써 
해결해 주는 서버 node.js 미들웨어 

> https://github.com/bripkens/connect-history-api-fallback

### copy-webpack-plugin

지정된 파일이나 디렉토리 전체를 빌드 디렉토리에 복사해 주는 webpack 플러그인 

> https://github.com/webpack-contrib/copy-webpack-plugin

### cross-spawn

node의 spawn 또는 spawnSync 를 크로스 플랫폼처리가 가능하도록 도와 주는 모듈

> https://github.com/moxystudio/node-cross-spawn

### css-loader

CSS 를 @import import/require 명령문에 사용가능하게 하는 webpack 로더 플러그 인

### diacritics

문자열에서 발음 구별 기호를 제거하고 해당 문자열로 변환해 주는 모듈 

> https://github.com/andrewrk/node-diacritics

### docsearch.js

Algolia는 Algolia DocSearch라는 무료 제품
오픈 소스 인 docsearch crawler를 사용하여 
Algolia 계정으로 웹 사이트들을 크롤링 한 결과를 표시할 수 있도록 도와 주는 모듈 

> https://github.com/algolia/docsearch

### escape-html

& 와 같은 특수 문자를 HTML 에서 사용하도록 도와 주는 모듈 

> https://github.com/component/escape-html

### eslint

자바스크립트의 문법 에러와 코딩 룰을 검사해 주는 모듈

> https://github.com/eslint/eslint

### eslint-plugin-jest

Jest 용 eslint 플러그 인

> https://github.com/jest-community/eslint-plugin-jest

### eslint-plugin-vue-libs

vue 자체 라이브러리 용 eslint 

> https://github.com/vuejs/eslint-plugin-vue-libs

### file-loader

파일을 빌드 디렉토리에 복사해 주는 webpack 로더

> https://github.com/webpack-contrib/file-loader

### fs-extra

node 의 fs 모듈을 좀 더 좋게 확장한 모듈 

> https://github.com/jprichardson/node-fs-extra

### globby

fast-glob 을 좀 더 쓰기 편하게 확장한 모듈 
glob는 파일들의 목록을 뽑을 때 사용하는 것으로 '*.txt" 같은 처리를 의미함 

> https://github.com/sindresorhus/globby

### gray-matter

문자열이나 파일에서 YAML 포맷으로 선언된 내용을 JSON 객제로 바꾸어 준다.

다음과 같은 내용이 있다면 

    ---
    title: Hello
    slug: home
    ---
    <h1>Hello world!</h1>

다음과 같은 오브젝트로 변환해 준다. 

    {
        content: '<h1>Hello world!</h1>',
        data: { 
            title: 'Hello', 
            slug: 'home' 
        }
    }

> https://github.com/jonschlinkert/gray-matter

### jest

페이스북에 만든 테스트 프레임워크

> https://github.com/facebook/jest

### jest-serializer-vue

jest 에서 테스트 비교를 위해 마운트된 컴포넌트를 미리 단순하게 직렬화 해주는 모듈
** 직렬화란 연속된 바이트 데이터과 같은 형태로 만든다는 의미...

> https://github.com/eddyerburgh/jest-serializer-vue

### js-yaml

YAML 1.2 문법을 자바스크립트에서 사용하도록 해석거사 생성해 주는 모듈

> https://github.com/nodeca/js-yaml

### koa-connect

Express 멤버들이 만든 Express 보다 가볍고 공개 버전안 KOA 용 connect 미들웨어

> https://github.com/vkurchatkin/koa-connect

### koa-mount

KOA 마운트 모듈 

> https://github.com/koajs/mount

### koa-range

KOA 레인지 모듈 

> https://github.com/koajs/koa-range 

### koa-static

KOA 스테틱 파일 서버 미들웨어 모듈 

> https://github.com/koajs/static

### lint-staged

staged된 파일들을 lint 해주는 도구 
Husky와 같이 쓰면 staged된 파일들에 대해서 특정 작업을 수행할 수 있음

> https://github.com/okonet/lint-staged

### loader-utils

webpack 로더를 위한 유틸리티 모듈 

> https://github.com/webpack/loader-utils

### lodash.throttle

node 용으로 매 밀리세컨드마다 최대 한 번만 호출될 수 있도록 Throttle된 함수를 만들어 주는 모듈

> https://github.com/lodash/lodash

### lru-cache

가장 오래 전에 사용되지 않은 항목을 삭제하는 캐시 객체 관리 모듈

LRU란, Least Recently Used 의 줄임말로, 특정 용량이 지정되어있을때,
사용(set 또는 get)한지가 가장 오래된 element를 자동으로 캐시에서 제거해 나가며,
데이터를 캐싱할 수 있도록 해주는 자료구조

> https://github.com/isaacs/node-lru-cache

### markdown-it

마크 다운 파서 

> https://github.com/markdown-it/markdown-it

### markdown-it-anchor

markdown-it을 위한 헤더 링크 처리
markdown-it-table-of-contents 와 연동됨

> https://github.com/valeriangalliat/markdown-it-anchor

### markdown-it-container

markdown-it 의 커스텀 블럭을 처리하기 위한 플러그인 

> https://github.com/markdown-it/markdown-it-container

### markdown-it-emoji

markdown-it에서 이모지 처리 

> https://github.com/markdown-it/markdown-it-emoji

### markdown-it-table-of-contents

markdown-it-anchor와 연동되어 TOC (table of contents) 처리 

> https://github.com/Oktavilla/markdown-it-table-of-contents

### mini-css-extract-plugin

CSS를 별도의 파일로 추출허눈 webpack 플러그 인

> https://github.com/webpack-contrib/mini-css-extract-plugin

### nprogress

AJAX 를 이용하는 어플리키에션을 위한 간단한 진행바

> https://github.com/rstacruz/nprogress

### optimize-css-assets-webpack-plugin

css 를 최적화 하여 최소화 시키는 webpack 플러그 인

> https://github.com/NMFR/optimize-css-assets-webpack-plugin

### portfinder

사용되지 않은 포트 번호를 얻어 온다. 

> https://github.com/indexzero/node-portfinder

### postcss-loader

PostCSS 를 webpack 에서 사용 할 수 있도록 하는 로더

PostCSS 란 CSS 를 처리하기 위한 webpack 도는 gulp 같은 프레임워크 이다. 
다양한 PostCSS 용 플러그인을 사용하여 css 를 처리한다.

> https://github.com/postcss/postcss-loader

### prismjs

신텍스 하이라이트 모듈 

> https://github.com/PrismJS/prism

### register-service-worker

간단한 서비스 워커 처리기 

> https://github.com/yyx990803/register-service-worker

### semver

시맨틱 버젼 2.0.0

>  https://semver.org/  
>  https://github.com/npm/node-semver  

### stylus

CSS 를 편하게 사용할 수 있도록 하는 stylus 문법 컴파일 모듈 

> https://github.com/stylus/stylus

### stylus-loader

stylus 문법 처리를 위한 webpack 용 로더

> https://github.com/shama/stylus-loader

### toml

JSON 또는 YAML과 유사한 데이터 표현 파일 포맷이다. 

> https://github.com/toml-lang/toml

### url-loader

작은 이미지나 글꼴 파일은 복사하지 않고 base64 문자열 형태로 변환하여 번들 파일에 추가함

> https://github.com/webpack-contrib/url-loader/

### vue

vue.js  처리 모듈 

> https://github.com/vuejs/vue

### @vue/babel-preset-app

VUE 를 위한 바벨 프리셋

> https://github.com/vuejs/babel-preset-vue-app

### vue-jest

jest  테스트 에서 vue를 지원하기 위한 모듈

> https://github.com/vuejs/vue-jest

### vue-loader

VUE 의 싱크 파일 컴포넌트 를 지원하기 위한 webpack 로더 

> https://github.com/vuejs/vue-loader

### vue-router

VUE 라우터 모듈 

> https://github.com/vuejs/vue-router

### vue-server-renderer

node.js 서버에서 vue 2.0 을 렌더링하도록 지원하는 모듈이다.

> https://github.com/vuejs/vue/tree/dev/packages/vue-server-renderer

### vue-template-compiler

런타임 컴파일 오버 헤드 및 콘텐츠 보안 정책(CSP) 제한을 피하기 위해 
Vue 2.0 템플릿을 렌더링 함수로 사전 컴파일하는 데 사용하는 모듈 

> https://github.com/vuejs/vue

### vuepress-html-webpack-plugin

vue 를 위한 webpack 용 html 플러그 인 

> https://www.npmjs.com/package/vuepress-html-webpack-plugin  
> https://github.com/jantimon/html-webpack-plugin

### @vue/test-utils

vue 테스트를 위한 유틸리티 

> https://github.com/vuejs/vue-test-utils

### webpack

webpack 모듈

> https://github.com/webpack/webpack

### webpack-chain

webpack 체인 모듈

> https://github.com/neutrinojs/webpack-chain

### webpack-merge

webpack 머지 모듈

> https://github.com/survivejs/webpack-merge

### webpack-serve

웹팩 개발 서버 패키지

> https://github.com/webpack-contrib/webpack-serve

### webpackbar

웹팩 텍스트 진행도 표시 유틸리티

> https://github.com/nuxt/webpackbar

![](https://github.com/nuxt/webpackbar/blob/master/assets/screen1.png?raw=true)
    
### workbox-build

Service Worker 생성툴 

> https://developers.google.com/web/tools/workbox/modules/workbox-build

### yorkie

husky 를 약간 수정한 포크이다. 
husky 는 깃 훅을 편하게 작성할 수 있게 도와주는 도구로 잘못된 깃트 커밋과 푸쉬를 막아준다. 

> https://github.com/yyx990803/yorkie  
> https://github.com/typicode/husky  
