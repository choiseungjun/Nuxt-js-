# Nuxt JS 시작하기 🧑‍💻 

## Nuxt JS 란?
  
    Nuxt.js는 Vue.js 애플리케이션을 만들기 위한 Framework이며,   
    보다 강력한 Application을 좀 더 손쉽게 만들 수 있으며 Server-Side-Rendering을 지원한다.

###### * 서버 사이드 렌더링이란, 서버에서 페이지를 그려 클라이언트(브라우저)로 보낸 후 화면에 표시하는 기법을 의미한다. 
###### * 클라이언트 사이드 렌더링은 페이지의 내용을 브라우저에서 그리고 서버 사이드 렌더링은 서버에서 페이지의 내용을 다 그려서 브라우저로 던져준다.

깃헙 : https://github.com/nuxt/nuxt.js   
공식 사이트 : https://ko.nuxtjs.org/

### Nuxt 장점 
- Nuxt.js 설치만으로 이미 scaffolding(프로젝트 구조화)을 해주므로 딱히 프로젝트 구조에 대해서 고민할 필요가 없다.   
- Vue.js 하나하나 잡아줘야 할 라우팅을 Nuxt.js에서 파일을 생성하는 것만으로 라우팅을 자동으로 생성해 준다.   
- layout, store, middleware와 같은 요소들을 이미 구분을 지어주고 필요한 항목들을 처리해주기 때문에 순전히 개발에만 집중하면 된다.   
- Server-Side-Rendering에 필요한 요소가 이미 준비가 되어있다.   
- webpack을 통한 빌드 시스템이 이미 구현되어 있다. 그저 npm run만 해주면 된다.  
- **일반적인 SPA 개발은, 검색 엔진에서 노출되지 않아 조회가 힘들다. 하지만 Nuxt를 이용하게 되면 서버사이드렌더링으로 화면을 보여주기 때문에, 검색엔진 봇이 화면들을 잘 긁어갈 수 있다. 따라서 SPA로 개발하더라도 SEO(검색 엔진 최적화)를 걱정하지 않아도 된다.**

## 1. Nuxt 시작하기

**1.1 Nuxt starter 템플릿 사용하기**  
>  starter 템플릿을 .zip로 다운받아 사용하거나, vue-cli로 설치한다.  

	
###### Vue cli 설치
    npm i -g @vue/cli   
    npm i -g @vue/cli-init
    
**1.2 프로젝트 실행하기**

	$ cd <project-name>
	$ npm install
	$ npm run dev

http://localhost:3000/

<br />
    
    
## 2. 처음부터 시작하기   
>  Nuxt를 처음 부터 시작하기 위해서는 한개의 파일의 한개의 디렉토리가 필요하다.

	$ mkdir <project-name>
	$ cd <project-name>


**1.2 프로젝트 생성하기**

    npx create-nuxt-app <project-name>
    npm init nuxt-app <project-name>
    yarn create nuxt-app <project-name>

**1.3 프로젝트 실행하기**
  
>  Successfully created project [프로젝트명] 메세지 출력

	cd <project-name>
	npm run dev

http://localhost:3000/

###### * Nuxt.js는 pages 디렉토리 내의 파일 변경 사항을 수신하므로 새 페이지를 추가 할 때 응용 프로그램을 다시 시작할 필요가 없습니다.



## 2. Nuxt JS 디렉토리 구조

	Nuxt.js의 기본 템플릿을 설치 하였다면 이미 스캐폴딩이 되어 있다.

##### assets
######  LESS, SASS, Javascript 와 같은 컴파일 되지 않은 파일들이 포함된다.

##### components
###### 애플리케이션에서 사용될 컴포넌트들을 포함하며 해당 경로에 위치된 컴포넌트들은 Nuxt.js의 비동기 데이터 함수인 asyncData또는 fetch를 사용할 수 없다.

##### content
###### content는 @nuxt/content 모듈을 사용하여 애플리케이션을 확장할 수 있다. Markdown, JSON, YAML, XML, CSV와 같은 파일을 가져오고 관리할 수 있다. nuxt/contents에서 더 많은 정보를 확인해보자.

##### layouts
###### 애플리케이션 전체에 대한 레이아웃을 포함한다. 기본으로 default.vue가 생성되어 있을 것이고 상황에 맞게 layout을 생성할 수 있다. 해당 디렉토리는 이름을 변경할 수 없다.

##### middleware
###### 애플리케이션에서 사용될 middleware를 포함한다. middleware는 페이지 또는 레이아웃이 렌더링 되기 전에 실행이 되며, middleware를 페이지나 레이아웃에 바인딩하였다면 해당 페이지나 레이아웃이 실행되기 전에 매번 실행된다.

##### module
###### Nuxt Module은 Nuxt 프레임워크의 핵심 기능을 확장하고 통합 및 추가할 수 있다. 사용자가 직접 모듈을 작성할 수 있으며 Nuxt 커뮤니티에 이미 많은 모듈이 공개되어있다.

##### pages
###### 실제 애플리케이션의 페이지 구성을 포함하며 해당 디렉토리의 구조에 따라 router가 자동으로 생성된다. 해당 디렉토리는 이름을 변경할 수 없다.

##### plugins
###### 애플리케이션에 바인딩 될 외부 혹은 내부 plugins를 포함한다.plugins는 애플리케이션이 인스턴스 화 되기 전에 실행하며 전역적으로 구성 요소를 등록하고 함수 또는 상수를 삽입할 수 있다.

##### static
###### 해당 디렉토리는 정적인 파일들을 포함한다. 구성에 따라서 html, Javascript 파일도 포함 시킬 수 있다. 해당 디렉토리는 이름을 변경할 수 없다.

##### store
###### 애플리케이션에서 사용될 vuex store 파일들을 포함한다. 기본적으로 비활성화 상태이고 store 디렉토리에 index.js 파일을 작성하면 store가 활성화된다. 구성에 따라서 모듈 형태의 store를 형성할 수 있다. 해당 디렉토리는 이름을 변경할 수 없다.


## 3. 라우팅

	Nuxt.js pages 디렉토리 내의 Vue 파일 구조를 기반으로 vue-router 설정을 자동으로 생성한다.
	
**3.1 기본 라우팅**

**1. pages 폴더내 vue파일 생성시**

```` js
pages/
--| user/
-----| index.vue
-----| one.vue
--| index.vue
````

**2. .nuxt - router.js 파일내에 아래와 같이 라우터 자동 생성**

```` js
router: {
  routes: [
    {
      name: 'index',
      path: '/',
      component: 'pages/index.vue'
    },
    {
      name: 'user',
      path: '/user',
      component: 'pages/user/index.vue'
    },
    {
      name: 'user-one',
      path: '/user/one',
      component: 'pages/user/one.vue'
    }
  ]
}
```` 

**3.2 동적 라우팅**


	파라메터가 있는 동적 라우트를 정의하기 위해서는 앞에 밑줄이 붙은 .vue 파일이나 폴더를 정의해야한다.
	
```` js
pages/
--| _slug/
-----| comments.vue
-----| index.vue
--| users/
-----| _id.vue
--| index.vue


아래와 같이 생성

router: {
  routes: [
    {
      name: 'index',
      path: '/',
      component: 'pages/index.vue'
    },
    {
      name: 'users-id',
      path: '/users/:id?',
      component: 'pages/users/_id.vue'
    },
    {
      name: 'slug',
      path: '/:slug',
      component: 'pages/_slug/index.vue'
    },
    {
      name: 'slug-comments',
      path: '/:slug/comments',
      component: 'pages/_slug/comments.vue'
    }
  ]
}

````

**3.3 트랜지션**
	Nuxt.js는 경로 전환 과정에서 <transition> 컴포넌트를 사용해 놀라운 트랜지션/애니메이션을 만들어냅니다.
	
	
###### * 모든 페이지에 페이드 애니메이션을 추가하기 위해서는 모든 라우트에 사용될 CSS 파일을 작성해야 한다. 
	따라서 assets 폴더에 CSS 파일을 만드는 것부터 시작한다.  → 전역 css 파일인 assets/main.css
	
```` css
.page-enter-active, .page-leave-active {
  transition: opacity .5s;
}
.page-enter, .page-leave-to {
  opacity: 0;
}
````
	
이를 nuxt.config.js 파일에 추가합니다:

```` js
module.exports = {
  css: [
    'assets/main.css'
  ]
}
````
	
	
## 4.레이아웃

	Nuxt.js를 사용하면 layouts 폴더에 레이아웃을 추가함으로써 메인 레이아웃을 확장하거나 사용자 정의 레이아웃을 만들 수 있다.
	메인 레이아웃을 확장하려면 layouts/default.vue 파일을 추가하며, 페이지 컴포넌트를 레이아웃에 렌더링하기 위해서 꼭 <nuxt/> 태그를 작성해야만 한다.

	<template>
	  <nuxt/>
	</template>
	
## 5.에러 페이지
	
	에러 페이지를 커스터마이징하려면 layouts/error.vue 파일을 추가한다.
	이 레이아웃은 <nuxt/> 태그를 포함하지 않으며, 404나 500 에러가 발생했을 때 이 레이아웃은 컴포넌트로 자동 연결된다.


	

	<template>
  <h1 class="red">Hello {{ name }}!</h1>
</template>

<script>
export default {
  asyncData (context) {
    // called every time before loading the component
    return { name: 'World' }
  },
  fetch () {
    // The fetch method is used to fill the store before rendering the page
  },
  head () {
    // Set Meta Tags for this Page
  },
  // and more functionality to discover
  ...
}
</script>

<style>
.red {
  color: red;
}
</style>
	
	속성	설명
asyncData	가장 중요한 키며 비동기적으로 만들 수 있고, 첫 번째 인자로 전달 받을 수도 있습니다. 자세한 내용 및 어떻게 동작하는 지는 이곳에서 확인합니다.
fetch	페이지가 렌더링되기 전에 스토어를 채우기위해 사용되며, 구성 요소 데이터를 설정하지 않는다는 점을 제외하면 데이터 메소드와 같습니다. 자세한 내용은 이곳에서 확인합니다.
head	현재 페이지에 대한 특정 메타 태그를 설정하려면 이곳에서 확인합니다.
layout	layouts 폴더에 정의된 레이아웃을 지정할 수 있습니다. 자세한 내용은 이곳에서 확인합니다.
transition	페이지에 대한 특정 트랜지션을 설정합니다. 자세한 내용은 이곳에서 확인합니다.
scrollToTop	기본값은 false 입니다. 페이지를 렌더링하기 전에 페이지를 맨 위로 스크롤할 것인지를 나타내며, 중첩 라우트를 위해 사용됩니다. 자세한 내용은 이곳에서 확인합니다.
validate	동적 라우트에 대한 유효성을 검사합니다. 자세한 내용은 이곳에서 확인합니다.
middleware	이 페이지에 대한 미들웨어를 설정하면, 미들웨어는 페이지를 렌더링하기 전에 호출되며, 자세한 내용은 이곳에서 확인합니다.
	
	

## Nuxt.js는 headers 와 html attributes 를 갱신하기 위해서 vue-meta를 사용합니다. (Nuxt.js는 vue-meta를 아래의 옵션으로 구성합니다.)

### 기본 메타 태그
Nuxt.js를 사용하면 nuxt.config.js에 head 속성을 사용함으로써 기본 메타를 정의할 수 있습니다:

사용자 정의 구글 폰트와 사용자 정의 뷰포트를 설정하는 예시입니다:

	head: {
	  meta: [
	    { charset: 'utf-8' },
	    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
	  ],
	  link: [
	    { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Roboto' }
	  ]
	}
