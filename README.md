# NUXT JS 시작하기 🧑‍💻 

## NUXT JS 란?
  
    Nuxt.js는 Vue.js 애플리케이션을 만들기 위한 Framework이며,   
    보다 강력한 Application을 좀 더 손쉽게 만들 수 있으며 Server-Side-Rendering을 지원한다.

###### * 서버 사이드 렌더링이란, 서버에서 페이지를 그려 클라이언트(브라우저)로 보낸 후 화면에 표시하는 기법을 의미한다. 
###### * 클라이언트 사이드 렌더링은 페이지의 내용을 브라우저에서 그리고 서버 사이드 렌더링은 서버에서 페이지의 내용을 다 그려서 브라우저로 던져준다.

깃헙 : https://github.com/nuxt/nuxt.js   
공식 사이트 : https://ko.nuxtjs.org/   

### Nuxt.js 장점 
- Nuxt.js 설치만으로 이미 scaffolding(프로젝트 구조화)을 해주므로 딱히 프로젝트 구조에 대해서 고민할 필요가 없다.   
- Vue.js 하나하나 잡아줘야 할 라우팅을 Nuxt.js에서 파일을 생성하는 것만으로 라우팅을 자동으로 생성해 준다.   
- layout, store, middleware와 같은 요소들을 이미 구분을 지어주고 필요한 항목들을 처리해주기 때문에 순전히 개발에만 집중하면 된다.   
- Server-Side-Rendering에 필요한 요소가 이미 준비가 되어있다.   
- webpack을 통한 빌드 시스템이 이미 구현되어 있다. 그저 npm run만 해주면 된다.  
- **일반적인 SPA 개발은, 검색 엔진에서 노출되지 않아 조회가 힘들다. 하지만 Nuxt를 이용하게 되면 서버사이드렌더링으로 화면을 보여주기 때문에, 검색엔진 봇이 화면들을 잘 긁어갈 수 있다. 따라서 SPA로 개발하더라도 SEO(검색 엔진 최적화)를 걱정하지 않아도 된다.**


## 1. NUXT 시작하기

**1. Vue cli 설치**

    npm i -g @vue/cli   
    npm i -g @vue/cli-init

**2. 프로젝트 생성하기**

    npx create-nuxt-app <project-name>
    npm init nuxt-app <project-name>
    yarn create nuxt-app <project-name>

**3. 프로젝트 실행하기**
  
>  Successfully created project [프로젝트명] 메세지 출력

    To get started:
	cd [디렉토리명]
	npm run dev

    To build & start for production:
	cd [디렉토리명]
	npm run build
	npm run start

    To test:
	cd [디렉토리명]
	npm run test

