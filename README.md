# Nuxt JS ์์ํ๊ธฐ ๐งโ๐ป 

## Nuxt JS ๋?
  
    Nuxt.js๋ Vue.js ์ ํ๋ฆฌ์ผ์ด์์ ๋ง๋ค๊ธฐ ์ํ Framework์ด๋ฉฐ,   
    ๋ณด๋ค ๊ฐ๋ ฅํ Application์ ์ข ๋ ์์ฝ๊ฒ ๋ง๋ค ์ ์์ผ๋ฉฐ Server-Side-Rendering์ ์ง์ํ๋ค.

###### * ์๋ฒ ์ฌ์ด๋ ๋ ๋๋ง์ด๋, ์๋ฒ์์ ํ์ด์ง๋ฅผ ๊ทธ๋ ค ํด๋ผ์ด์ธํธ(๋ธ๋ผ์ฐ์ )๋ก ๋ณด๋ธ ํ ํ๋ฉด์ ํ์ํ๋ ๊ธฐ๋ฒ์ ์๋ฏธํ๋ค. 
###### * ํด๋ผ์ด์ธํธ ์ฌ์ด๋ ๋ ๋๋ง์ ํ์ด์ง์ ๋ด์ฉ์ ๋ธ๋ผ์ฐ์ ์์ ๊ทธ๋ฆฌ๊ณ  ์๋ฒ ์ฌ์ด๋ ๋ ๋๋ง์ ์๋ฒ์์ ํ์ด์ง์ ๋ด์ฉ์ ๋ค ๊ทธ๋ ค์ ๋ธ๋ผ์ฐ์ ๋ก ๋์ ธ์ค๋ค.

๊นํ : https://github.com/nuxt/nuxt.js   
๊ณต์ ์ฌ์ดํธ : https://ko.nuxtjs.org/

### Nuxt ์ฅ์  
- Nuxt.js ์ค์น๋ง์ผ๋ก ์ด๋ฏธ scaffolding(ํ๋ก์ ํธ ๊ตฌ์กฐํ)์ ํด์ฃผ๋ฏ๋ก ๋ฑํ ํ๋ก์ ํธ ๊ตฌ์กฐ์ ๋ํด์ ๊ณ ๋ฏผํ  ํ์๊ฐ ์๋ค.   
- Vue.js ํ๋ํ๋ ์ก์์ค์ผ ํ  ๋ผ์ฐํ์ Nuxt.js์์ ํ์ผ์ ์์ฑํ๋ ๊ฒ๋ง์ผ๋ก ๋ผ์ฐํ์ ์๋์ผ๋ก ์์ฑํด ์ค๋ค.   
- layout, store, middleware์ ๊ฐ์ ์์๋ค์ ์ด๋ฏธ ๊ตฌ๋ถ์ ์ง์ด์ฃผ๊ณ  ํ์ํ ํญ๋ชฉ๋ค์ ์ฒ๋ฆฌํด์ฃผ๊ธฐ ๋๋ฌธ์ ์์ ํ ๊ฐ๋ฐ์๋ง ์ง์คํ๋ฉด ๋๋ค.   
- Server-Side-Rendering์ ํ์ํ ์์๊ฐ ์ด๋ฏธ ์ค๋น๊ฐ ๋์ด์๋ค.   
- webpack์ ํตํ ๋น๋ ์์คํ์ด ์ด๋ฏธ ๊ตฌํ๋์ด ์๋ค. ๊ทธ์  npm run๋ง ํด์ฃผ๋ฉด ๋๋ค.  
- **์ผ๋ฐ์ ์ธ SPA ๊ฐ๋ฐ์, ๊ฒ์ ์์ง์์ ๋ธ์ถ๋์ง ์์ ์กฐํ๊ฐ ํ๋ค๋ค. ํ์ง๋ง Nuxt๋ฅผ ์ด์ฉํ๊ฒ ๋๋ฉด ์๋ฒ์ฌ์ด๋๋ ๋๋ง์ผ๋ก ํ๋ฉด์ ๋ณด์ฌ์ฃผ๊ธฐ ๋๋ฌธ์, ๊ฒ์์์ง ๋ด์ด ํ๋ฉด๋ค์ ์ ๊ธ์ด๊ฐ ์ ์๋ค. ๋ฐ๋ผ์ SPA๋ก ๊ฐ๋ฐํ๋๋ผ๋ SEO(๊ฒ์ ์์ง ์ต์ ํ)๋ฅผ ๊ฑฑ์ ํ์ง ์์๋ ๋๋ค.**

## 1. Nuxt ์์ํ๊ธฐ

**1.1 Nuxt starter ํํ๋ฆฟ ์ฌ์ฉํ๊ธฐ**  
>  starter ํํ๋ฆฟ์ .zip๋ก ๋ค์ด๋ฐ์ ์ฌ์ฉํ๊ฑฐ๋, vue-cli๋ก ์ค์นํ๋ค.  

	
###### Vue cli ์ค์น
    npm i -g @vue/cli   
    npm i -g @vue/cli-init
    
**1.2 ํ๋ก์ ํธ ์คํํ๊ธฐ**

	$ cd <project-name>
	$ npm install
	$ npm run dev

http://localhost:3000/

<br />
    
    
## 2. ์ฒ์๋ถํฐ ์์ํ๊ธฐ   
>  Nuxt๋ฅผ ์ฒ์ ๋ถํฐ ์์ํ๊ธฐ ์ํด์๋ ํ๊ฐ์ ํ์ผ์ ํ๊ฐ์ ๋๋ ํ ๋ฆฌ๊ฐ ํ์ํ๋ค.

	$ mkdir <project-name>
	$ cd <project-name>


**1.2 ํ๋ก์ ํธ ์์ฑํ๊ธฐ**

    npx create-nuxt-app <project-name>
    npm init nuxt-app <project-name>
    yarn create nuxt-app <project-name>

**1.3 ํ๋ก์ ํธ ์คํํ๊ธฐ**
  
>  Successfully created project [ํ๋ก์ ํธ๋ช] ๋ฉ์ธ์ง ์ถ๋ ฅ

	cd <project-name>
	npm run dev

http://localhost:3000/

###### * Nuxt.js๋ pages ๋๋ ํ ๋ฆฌ ๋ด์ ํ์ผ ๋ณ๊ฒฝ ์ฌํญ์ ์์ ํ๋ฏ๋ก ์ ํ์ด์ง๋ฅผ ์ถ๊ฐ ํ  ๋ ์์ฉ ํ๋ก๊ทธ๋จ์ ๋ค์ ์์ํ  ํ์๊ฐ ์์ต๋๋ค.



## 2. Nuxt JS ๋๋ ํ ๋ฆฌ ๊ตฌ์กฐ

	Nuxt.js์ ๊ธฐ๋ณธ ํํ๋ฆฟ์ ์ค์น ํ์๋ค๋ฉด ์ด๋ฏธ ์ค์บํด๋ฉ์ด ๋์ด ์๋ค.

##### assets
######  LESS, SASS, Javascript ์ ๊ฐ์ ์ปดํ์ผ ๋์ง ์์ ํ์ผ๋ค์ด ํฌํจ๋๋ค.

##### components
###### ์ ํ๋ฆฌ์ผ์ด์์์ ์ฌ์ฉ๋  ์ปดํฌ๋ํธ๋ค์ ํฌํจํ๋ฉฐ ํด๋น ๊ฒฝ๋ก์ ์์น๋ ์ปดํฌ๋ํธ๋ค์ Nuxt.js์ ๋น๋๊ธฐ ๋ฐ์ดํฐ ํจ์์ธ asyncData๋๋ fetch๋ฅผ ์ฌ์ฉํ  ์ ์๋ค.

##### content
###### content๋ @nuxt/content ๋ชจ๋์ ์ฌ์ฉํ์ฌ ์ ํ๋ฆฌ์ผ์ด์์ ํ์ฅํ  ์ ์๋ค. Markdown, JSON, YAML, XML, CSV์ ๊ฐ์ ํ์ผ์ ๊ฐ์ ธ์ค๊ณ  ๊ด๋ฆฌํ  ์ ์๋ค. nuxt/contents์์ ๋ ๋ง์ ์ ๋ณด๋ฅผ ํ์ธํด๋ณด์.

##### layouts
###### ์ ํ๋ฆฌ์ผ์ด์ ์ ์ฒด์ ๋ํ ๋ ์ด์์์ ํฌํจํ๋ค. ๊ธฐ๋ณธ์ผ๋ก default.vue๊ฐ ์์ฑ๋์ด ์์ ๊ฒ์ด๊ณ  ์ํฉ์ ๋ง๊ฒ layout์ ์์ฑํ  ์ ์๋ค. ํด๋น ๋๋ ํ ๋ฆฌ๋ ์ด๋ฆ์ ๋ณ๊ฒฝํ  ์ ์๋ค.

##### middleware
###### ์ ํ๋ฆฌ์ผ์ด์์์ ์ฌ์ฉ๋  middleware๋ฅผ ํฌํจํ๋ค. middleware๋ ํ์ด์ง ๋๋ ๋ ์ด์์์ด ๋ ๋๋ง ๋๊ธฐ ์ ์ ์คํ์ด ๋๋ฉฐ, middleware๋ฅผ ํ์ด์ง๋ ๋ ์ด์์์ ๋ฐ์ธ๋ฉํ์๋ค๋ฉด ํด๋น ํ์ด์ง๋ ๋ ์ด์์์ด ์คํ๋๊ธฐ ์ ์ ๋งค๋ฒ ์คํ๋๋ค.

##### module
###### Nuxt Module์ Nuxt ํ๋ ์์ํฌ์ ํต์ฌ ๊ธฐ๋ฅ์ ํ์ฅํ๊ณ  ํตํฉ ๋ฐ ์ถ๊ฐํ  ์ ์๋ค. ์ฌ์ฉ์๊ฐ ์ง์  ๋ชจ๋์ ์์ฑํ  ์ ์์ผ๋ฉฐ Nuxt ์ปค๋ฎค๋ํฐ์ ์ด๋ฏธ ๋ง์ ๋ชจ๋์ด ๊ณต๊ฐ๋์ด์๋ค.

##### pages
###### ์ค์  ์ ํ๋ฆฌ์ผ์ด์์ ํ์ด์ง ๊ตฌ์ฑ์ ํฌํจํ๋ฉฐ ํด๋น ๋๋ ํ ๋ฆฌ์ ๊ตฌ์กฐ์ ๋ฐ๋ผ router๊ฐ ์๋์ผ๋ก ์์ฑ๋๋ค. ํด๋น ๋๋ ํ ๋ฆฌ๋ ์ด๋ฆ์ ๋ณ๊ฒฝํ  ์ ์๋ค.

##### plugins
###### ์ ํ๋ฆฌ์ผ์ด์์ ๋ฐ์ธ๋ฉ ๋  ์ธ๋ถ ํน์ ๋ด๋ถ plugins๋ฅผ ํฌํจํ๋ค.plugins๋ ์ ํ๋ฆฌ์ผ์ด์์ด ์ธ์คํด์ค ํ ๋๊ธฐ ์ ์ ์คํํ๋ฉฐ ์ ์ญ์ ์ผ๋ก ๊ตฌ์ฑ ์์๋ฅผ ๋ฑ๋กํ๊ณ  ํจ์ ๋๋ ์์๋ฅผ ์ฝ์ํ  ์ ์๋ค.

##### static
###### ํด๋น ๋๋ ํ ๋ฆฌ๋ ์ ์ ์ธ ํ์ผ๋ค์ ํฌํจํ๋ค. ๊ตฌ์ฑ์ ๋ฐ๋ผ์ html, Javascript ํ์ผ๋ ํฌํจ ์ํฌ ์ ์๋ค. ํด๋น ๋๋ ํ ๋ฆฌ๋ ์ด๋ฆ์ ๋ณ๊ฒฝํ  ์ ์๋ค.

##### store
###### ์ ํ๋ฆฌ์ผ์ด์์์ ์ฌ์ฉ๋  vuex store ํ์ผ๋ค์ ํฌํจํ๋ค. ๊ธฐ๋ณธ์ ์ผ๋ก ๋นํ์ฑํ ์ํ์ด๊ณ  store ๋๋ ํ ๋ฆฌ์ index.js ํ์ผ์ ์์ฑํ๋ฉด store๊ฐ ํ์ฑํ๋๋ค. ๊ตฌ์ฑ์ ๋ฐ๋ผ์ ๋ชจ๋ ํํ์ store๋ฅผ ํ์ฑํ  ์ ์๋ค. ํด๋น ๋๋ ํ ๋ฆฌ๋ ์ด๋ฆ์ ๋ณ๊ฒฝํ  ์ ์๋ค.


## 3. ๋ผ์ฐํ

	Nuxt.js pages ๋๋ ํ ๋ฆฌ ๋ด์ Vue ํ์ผ ๊ตฌ์กฐ๋ฅผ ๊ธฐ๋ฐ์ผ๋ก vue-router ์ค์ ์ ์๋์ผ๋ก ์์ฑํ๋ค.
	
**3.1 ๊ธฐ๋ณธ ๋ผ์ฐํ**

**1. pages ํด๋๋ด vueํ์ผ ์์ฑ์**

```` js
pages/
--| user/
-----| index.vue
-----| one.vue
--| index.vue
````

**2. .nuxt - router.js ํ์ผ๋ด์ ์๋์ ๊ฐ์ด ๋ผ์ฐํฐ ์๋ ์์ฑ**

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

**3.2 ๋์  ๋ผ์ฐํ**


	ํ๋ผ๋ฉํฐ๊ฐ ์๋ ๋์  ๋ผ์ฐํธ๋ฅผ ์ ์ํ๊ธฐ ์ํด์๋ ์์ ๋ฐ์ค์ด ๋ถ์ .vue ํ์ผ์ด๋ ํด๋๋ฅผ ์ ์ํด์ผํ๋ค.
	
```` js
pages/
--| _slug/
-----| comments.vue
-----| index.vue
--| users/
-----| _id.vue
--| index.vue


์๋์ ๊ฐ์ด ์์ฑ

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

**3.3 ํธ๋์ง์**
	Nuxt.js๋ ๊ฒฝ๋ก ์ ํ ๊ณผ์ ์์ <transition> ์ปดํฌ๋ํธ๋ฅผ ์ฌ์ฉํด ๋๋ผ์ด ํธ๋์ง์/์ ๋๋ฉ์ด์์ ๋ง๋ค์ด๋๋๋ค.
	
	
###### * ๋ชจ๋  ํ์ด์ง์ ํ์ด๋ ์ ๋๋ฉ์ด์์ ์ถ๊ฐํ๊ธฐ ์ํด์๋ ๋ชจ๋  ๋ผ์ฐํธ์ ์ฌ์ฉ๋  CSS ํ์ผ์ ์์ฑํด์ผ ํ๋ค. 
	๋ฐ๋ผ์ assets ํด๋์ CSS ํ์ผ์ ๋ง๋๋ ๊ฒ๋ถํฐ ์์ํ๋ค.  โ ์ ์ญ css ํ์ผ์ธ assets/main.css
	
```` css
.page-enter-active, .page-leave-active {
  transition: opacity .5s;
}
.page-enter, .page-leave-to {
  opacity: 0;
}
````
	
์ด๋ฅผ nuxt.config.js ํ์ผ์ ์ถ๊ฐํฉ๋๋ค:

```` js
module.exports = {
  css: [
    'assets/main.css'
  ]
}
````
	
	
## 4.๋ ์ด์์

	Nuxt.js๋ฅผ ์ฌ์ฉํ๋ฉด layouts ํด๋์ ๋ ์ด์์์ ์ถ๊ฐํจ์ผ๋ก์จ ๋ฉ์ธ ๋ ์ด์์์ ํ์ฅํ๊ฑฐ๋ ์ฌ์ฉ์ ์ ์ ๋ ์ด์์์ ๋ง๋ค ์ ์๋ค.
	๋ฉ์ธ ๋ ์ด์์์ ํ์ฅํ๋ ค๋ฉด layouts/default.vue ํ์ผ์ ์ถ๊ฐํ๋ฉฐ, ํ์ด์ง ์ปดํฌ๋ํธ๋ฅผ ๋ ์ด์์์ ๋ ๋๋งํ๊ธฐ ์ํด์ ๊ผญ <nuxt/> ํ๊ทธ๋ฅผ ์์ฑํด์ผ๋ง ํ๋ค.

	<template>
	  <nuxt/>
	</template>
	
## 5.์๋ฌ ํ์ด์ง
	
	์๋ฌ ํ์ด์ง๋ฅผ ์ปค์คํฐ๋ง์ด์งํ๋ ค๋ฉด layouts/error.vue ํ์ผ์ ์ถ๊ฐํ๋ค.
	์ด ๋ ์ด์์์ <nuxt/> ํ๊ทธ๋ฅผ ํฌํจํ์ง ์์ผ๋ฉฐ, 404๋ 500 ์๋ฌ๊ฐ ๋ฐ์ํ์ ๋ ์ด ๋ ์ด์์์ ์ปดํฌ๋ํธ๋ก ์๋ ์ฐ๊ฒฐ๋๋ค.


	

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
	
	์์ฑ	์ค๋ช
asyncData	๊ฐ์ฅ ์ค์ํ ํค๋ฉฐ ๋น๋๊ธฐ์ ์ผ๋ก ๋ง๋ค ์ ์๊ณ , ์ฒซ ๋ฒ์งธ ์ธ์๋ก ์ ๋ฌ ๋ฐ์ ์๋ ์์ต๋๋ค. ์์ธํ ๋ด์ฉ ๋ฐ ์ด๋ป๊ฒ ๋์ํ๋ ์ง๋ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
fetch	ํ์ด์ง๊ฐ ๋ ๋๋ง๋๊ธฐ ์ ์ ์คํ ์ด๋ฅผ ์ฑ์ฐ๊ธฐ์ํด ์ฌ์ฉ๋๋ฉฐ, ๊ตฌ์ฑ ์์ ๋ฐ์ดํฐ๋ฅผ ์ค์ ํ์ง ์๋๋ค๋ ์ ์ ์ ์ธํ๋ฉด ๋ฐ์ดํฐ ๋ฉ์๋์ ๊ฐ์ต๋๋ค. ์์ธํ ๋ด์ฉ์ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
head	ํ์ฌ ํ์ด์ง์ ๋ํ ํน์  ๋ฉํ ํ๊ทธ๋ฅผ ์ค์ ํ๋ ค๋ฉด ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
layout	layouts ํด๋์ ์ ์๋ ๋ ์ด์์์ ์ง์ ํ  ์ ์์ต๋๋ค. ์์ธํ ๋ด์ฉ์ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
transition	ํ์ด์ง์ ๋ํ ํน์  ํธ๋์ง์์ ์ค์ ํฉ๋๋ค. ์์ธํ ๋ด์ฉ์ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
scrollToTop	๊ธฐ๋ณธ๊ฐ์ false ์๋๋ค. ํ์ด์ง๋ฅผ ๋ ๋๋งํ๊ธฐ ์ ์ ํ์ด์ง๋ฅผ ๋งจ ์๋ก ์คํฌ๋กคํ  ๊ฒ์ธ์ง๋ฅผ ๋ํ๋ด๋ฉฐ, ์ค์ฒฉ ๋ผ์ฐํธ๋ฅผ ์ํด ์ฌ์ฉ๋ฉ๋๋ค. ์์ธํ ๋ด์ฉ์ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
validate	๋์  ๋ผ์ฐํธ์ ๋ํ ์ ํจ์ฑ์ ๊ฒ์ฌํฉ๋๋ค. ์์ธํ ๋ด์ฉ์ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
middleware	์ด ํ์ด์ง์ ๋ํ ๋ฏธ๋ค์จ์ด๋ฅผ ์ค์ ํ๋ฉด, ๋ฏธ๋ค์จ์ด๋ ํ์ด์ง๋ฅผ ๋ ๋๋งํ๊ธฐ ์ ์ ํธ์ถ๋๋ฉฐ, ์์ธํ ๋ด์ฉ์ ์ด๊ณณ์์ ํ์ธํฉ๋๋ค.
	
	

## Nuxt.js๋ headers ์ html attributes ๋ฅผ ๊ฐฑ์ ํ๊ธฐ ์ํด์ vue-meta๋ฅผ ์ฌ์ฉํฉ๋๋ค. (Nuxt.js๋ vue-meta๋ฅผ ์๋์ ์ต์์ผ๋ก ๊ตฌ์ฑํฉ๋๋ค.)

### ๊ธฐ๋ณธ ๋ฉํ ํ๊ทธ
Nuxt.js๋ฅผ ์ฌ์ฉํ๋ฉด nuxt.config.js์ head ์์ฑ์ ์ฌ์ฉํจ์ผ๋ก์จ ๊ธฐ๋ณธ ๋ฉํ๋ฅผ ์ ์ํ  ์ ์์ต๋๋ค:

์ฌ์ฉ์ ์ ์ ๊ตฌ๊ธ ํฐํธ์ ์ฌ์ฉ์ ์ ์ ๋ทฐํฌํธ๋ฅผ ์ค์ ํ๋ ์์์๋๋ค:

	head: {
	  meta: [
	    { charset: 'utf-8' },
	    { name: 'viewport', content: 'width=device-width, initial-scale=1' }
	  ],
	  link: [
	    { rel: 'stylesheet', href: 'https://fonts.googleapis.com/css?family=Roboto' }
	  ]
	}
