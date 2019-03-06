## Vue.js

### Getting started

#### Install

```
npm i -g vue-cli
```

* Create a project directory
```
mkdir ~/vueprojects && cd $_
```

* Create a simple project

```
vue init bootstrap-vue/webpack-simple small_project
```
* To create a large project
```
vue init bootstrap-vue/webpack large_project
```


> We will continue with the simple project for now

* Install npm dependencies

```
cd small_project
npm install
```

> This will install npm dependencies


* Add bootstrap for styling

```
npm i bootstrap-vue
```


* Start dev server

```
npm run dev
```

> This will start dev server on port 8080 or next available port (e.g. 8081/8082)

> Open http://localhost:8080 in browser to see the sample page.
> 

> After these initial steps the directory structure in your project folder will look like this:

├── README.md
├── index.html
├── package-lock.json
├── package.json
├── src
│   ├── App.vue
│   ├── assets
│   │   └── logo.png
│   └── main.js
└── webpack.config.js

> Here, App.vue and main.js are the primary files of interest. If we fire up our text editor and open main.js, we’ll see the following code, which imports the Bootstrap style sheet and Bootstrap-Vue:

```javascript
import Vue from 'vue';
import BootstrapVue from 'bootstrap-vue';
import App from './App.vue';
import 'bootstrap/dist/css/bootstrap.min.css';
import 'bootstrap-vue/dist/bootstrap-vue.css';

Vue.use(BootstrapVue);

new Vue({
  el: '#app',
  render: h => h(App),
})

```


