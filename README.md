# Kraft

## Project history

Kraft product about trade in materials and their calculation

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
 Dev env: "react-env --prefix UI_ENV --path './.env.development' -- vue-cli-service serve"
 Stage evn: "react-env --prefix UI_ENV --path './.env.stage' -- vue-cli-service serve"
 Prod env: "react-env --prefix UI_ENV --path './.env.prod' -- vue-cli-service serve"
```

### Compiles and minifies for production
```
"build": "vue-cli-service build"
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


## Modules


## Using libraries

The base libraries

* Vuelidate: https://www.npmjs.com/package/vuelidate
* Vue Toastification: https://www.npmjs.com/package/vue-toastification
* Axios https://github.com/axios/axios
* Vue https://v2.vuejs.org/v2/guide/installation.html
* Vuex https://vuex.vuejs.org/installation.html
* Vuetify https://vuetifyjs.com/en/getting-started/installation/
* Vuelidate https://www.npmjs.com/package/vuelidate
* VueRouter https://v3.router.vuejs.org/ru/installation.html
* VueDebounce https://www.npmjs.com/package/vue-debounce
* Vue-search-select https://github.com/moreta/vue-search-select
* Vue-moment https://www.npmjs.com/package/vue-moment
* Slider https://www.npmjs.com/package/swiper-vue2
* Vue-i18n https://www.npmjs.com/package/vue-i18n
* Vue moment https://www.npmjs.com/package/vue-moment
* vue-pincode-input https://www.npmjs.com/package/vue-pincode-input
* vue-search-select https://www.npmjs.com/package/vue-search-select

## Code Style

1) Component creates by type: <calculator-formatted-item >
![img.png](img.png)
2) Store (Vue.js)
    * name of mutations must start with "set". setUserById
    * name of actions must start with "load" loadAllEventTypes
    * name of getters must start with "get" Example: getProductListCatalog: state => state.productListCatalog
    * store should contain modules 

3) Constants, statuses should be cold by capitalized letters 
4) View must be in view directory
5) Components must be in components directory
6) Adapters must contain  functions generation API
7) API contains  functions generation API
8) Const contains static values
9) Assets contains images and icons

## Architecture

* VIEWS - directory for save pages. Example: Log, Home, UserList
* UTILS - utilitarian methods. Example: "api.js"
* ROUTE - create dynamic and static routes. Example: "/directory/catalog", 
* CONST - Save constants. Example: "OBJECT_STATUSES"
* COMPONENTS - Components allow us to split the UI into independent and reusable pieces, and think about each piece in isolation. Example: TablePagination
* ASSETS - directory for save images and icons
* API - configuration axios. Axios is a promise-based HTTP Client for node.js and the browser

## ICONS
Application has default icons of vuetify: https://fonts.google.com/icons?selected=Material+Icons:home
and custom icons: https://fonts.google.com/icons?selected=Material+Icons:home 

## PROJECT ENV
App has three environments. There are development, prod, stage.
To run the stage locally, you need to execute the command  "stage": "react-env --prefix UI_ENV --path './.env.stage' -- vue-cli-service serve",
To run the main (prod) locally, you need to execute the command "prod": "react-env --prefix UI_ENV --path './.env.prod' -- vue-cli-service serve"
To run the dev locally, you need to execute the command "dev": "react-env --prefix UI_ENV --path './.env.development' -- vue-cli-service serve"
Link stage is https://onliner2-staging.kraftds.com/#/
Link dev is http://88.198.193.193/

## BRANCHES
App has three branches: development, stage, main.
To perform the release, you need to merge the stage into the main branch.
You can work both with dev and with stage in terms of development. You also need a branch from dev/stage



