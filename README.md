# Nuxt JS 시작하기 🧑‍💻 

## Nuxt JS 란?
  
    Nuxt.js는 Vue.js 애플리케이션을 만들기 위한 Framework이며,   
    보다 강력한 Application을 좀 더 손쉽게 만들 수 있으며 Server-Side-Rendering을 지원한다.

###### * 서버 사이드 렌더링이란, 서버에서 페이지를 그려 클라이언트(브라우저)로 보낸 후 화면에 표시하는 기법을 의미한다. 
###### * 클라이언트 사이드 렌더링은 페이지의 내용을 브라우저에서 그리고 서버 사이드 렌더링은 서버에서 페이지의 내용을 다 그려서 브라우저로 던져준다.

깃헙 : https://github.com/nuxt/nuxt.js   
공식 사이트 : https://ko.nuxtjs.org/   , https://develop365.gitlab.io/nuxtjs-0.10.7-doc/ko/guide/

### Nuxt 장점 
- Nuxt.js 설치만으로 이미 scaffolding(프로젝트 구조화)을 해주므로 딱히 프로젝트 구조에 대해서 고민할 필요가 없다.   
- Vue.js 하나하나 잡아줘야 할 라우팅을 Nuxt.js에서 파일을 생성하는 것만으로 라우팅을 자동으로 생성해 준다.   
- layout, store, middleware와 같은 요소들을 이미 구분을 지어주고 필요한 항목들을 처리해주기 때문에 순전히 개발에만 집중하면 된다.   
- Server-Side-Rendering에 필요한 요소가 이미 준비가 되어있다.   
- webpack을 통한 빌드 시스템이 이미 구현되어 있다. 그저 npm run만 해주면 된다.  
- **일반적인 SPA 개발은, 검색 엔진에서 노출되지 않아 조회가 힘들다. 하지만 Nuxt를 이용하게 되면 서버사이드렌더링으로 화면을 보여주기 때문에, 검색엔진 봇이 화면들을 잘 긁어갈 수 있다. 따라서 SPA로 개발하더라도 SEO(검색 엔진 최적화)를 걱정하지 않아도 된다.**


## 1. Nuxt 시작하기

**1.1 Nuxt starter 템플릿 사용하기


Vue cli 설치**

    npm i -g @vue/cli   
    npm i -g @vue/cli-init
    

**1.2 프로젝트 생성하기**

    npx create-nuxt-app <project-name>
    npm init nuxt-app <project-name>
    yarn create nuxt-app <project-name>

**1.3 프로젝트 실행하기**
  
>  Successfully created project [프로젝트명] 메세지 출력

	cd <project-name>
	npm run dev
	(NUXT 디렉토리가 자동 생성)

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

