# Onliner 2.0 Application

## Table of Contents
- [Onliner 2.0 Application](#onliner-20-application)
  - [Project history](#project-history)
  - [Project setup](#project-setup)
    - [Compiles and hot-reloads for development](#Compiles-and-hot-reloads-for-development)
    - [Compiles and minifies for production](#Compiles-and-minifies-for-production)
    - [Customize configuration](#Customize-configuration)
  - [Technologies](#technologies)
    - [Application Frameworks](#application-frameworks)
    - [Using libraries](#using-libraries)
  - [Code Style](#code-style)
  - [Architecture](#architecture)
  - [Icons](#icons)
  - [Project ENV](#project-env)
  - [Branches](#branches)
  - [Design](#design)
  - [Additional Documentation](#additional-documentation)
## Project history

> Onliner 2.0 is a B2B system that enables the collaboration between Kraft Company and its clients.
> Users can register, create and manage companies, handle objects, browse products, and make orders.
> The system includes a multifunctional flexible configurator tool for creating smart product catalogs for its clients 
> and distributors.  Which further allows customers to select available products or their types using an already 
> configured calculator.  Based on this choice, the calculator will calculate and select a list of necessary basic and
> additional goods in the right quantity for certain client needs. Based on miscalculations it supports order creation, 
> and allows users to define preferred shipment methods. Streamlining these processes, the platform enhances the
> efficiency of business interactions for both Kraft Company and its clients.

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

## Technologies

### Application Frameworks

* [Vue](https://v2.vuejs.org/v2/guide/installation.html) - framework for building user interfaces

* [Vuetify](https://vuetifyjs.com/en/getting-started/installation/) - Vue Component Framework. A no design skills required open source UI library with beautifully handcrafted collection of pre-made components which enable developers to create small modules to be used and re-used throughout an application

### Using libraries

* [Vuex](https://vuex.vuejs.org/installation.html) - a centralized store for all the components in an application, with rules ensuring that the state can only be mutated in a predictable fashion.

* [VueRouter](https://v3.router.vuejs.org/ru/installation.html) - configurable and convenient routing 

* [Axios](https://github.com/axios/axios) - isomorphic promise-based HTTP Client

* [Vue-i18n](https://www.npmjs.com/package/vue-i18n) - component-oriented internationalization plugin

* [Vuelidate](https://www.npmjs.com/package/vuelidate) - lightweight model-based validation

* [reCAPTCHA](https://developers.google.com/recaptcha/docs/v3) - uses an advanced risk analysis engine and adaptive challenges to keep malicious software from engaging in abusive activities on the website, fake users will be blocked. reCAPTCHA v3 returns a score for each request without user friction. The score is based on interactions with the site

* [Vue Toastification](https://www.npmjs.com/package/vue-toastification) - allows adding notifications (toasts) in a convenient and appealing way

* [VueDebounce](https://www.npmjs.com/package/vue-debounce) - dynamic debouncing for input based requests

* [Vue-moment](https://www.npmjs.com/package/vue-moment) - parse, validate, manipulate, and display dates and times

* [Google maps](https://developers.google.com/maps/documentation) - the Google Maps JavaScript API use script tag  to include into the application. It dynamically loads the API asynchronously for better performance. Implemented multi-colored markers to display different categories of objects. It is also possible to search for an address by a marker on the map. What can be reused in any component of the application

* [Overlapping Marker Spiderfier](https://www.npmjs.com/package/overlapping-marker-spiderfier) - makes map markers in the Google Maps API behave in that Google Earth way (minus the animation). Small numbers of markers (yes, up to 8) spiderfy into a circle. Larger numbers fan out into a more space-efficient spiral

* [Slider](https://www.npmjs.com/package/swiper-vue2)

## Code Style

1) Store (Vue.js)
    * name of mutations must start with "set". setUserById
    * name of actions must start with "load" loadAllEventTypes
    * name of getters must start with "get" Example: getProductListCatalog: state => state.productListCatalog
    * store should contain modules 

2) Constants, statuses should be cold by capitalized letters 
3) View must be in view directory
4) Components must be in components directory
5) Adapters must contain  functions generation API
6) API contains  functions generation API
7) Const contains static values
8) Assets contains images and icons

## Architecture

* **views** - directory for save pages. Example: Log, Home, UserList
* **utils** - utilitarian methods. Example: "api.js"
* **router** - create dynamic and static routes. Example: "/directory/catalog", 
* **i18n** - contains from the i18n configuration file and the default localization file, 
* **vuetify** - contains from the vuetify configuration file, 
* **const** - Save constants. Example: "OBJECT_STATUSES"
* **components** - Components allow us to split the UI into independent and reusable pieces, and think about each piece in isolation. Example: TablePagination
* **assets** - directory for save images and icons
* **api** - configuration axios. Axios is a promise-based HTTP Client for node.js and the browser

## Icons
Application has default icons of vuetify: https://fonts.google.com/icons?selected=Material+Icons:home
and custom icons: https://fonts.google.com/icons?selected=Material+Icons:home 

## Project ENV
App has three environments

 - **development** - an environment for implementing new features, debugging, and initially testing them 

  To run the dev locally, you need to execute the command "dev": "react-env --prefix UI_ENV --path './.env.development' -- vue-cli-service serve"

  Link dev is http://88.198.193.193/

 - **stage** - as close as possible to the production environment, it allows to test or demonstrate the performance of a product version before deploying it to the production environment

  To run the stage locally, you need to execute the command  "stage": "react-env --prefix UI_ENV --path './.env.stage' -- vue-cli-service serve"

  Link stage is https://onliner2-staging.kraftds.com/#/

 - **prod** - is a real-world working environment in which the latest versions of the product, after all testing has been completed and all bugs have been resolved, are delivered to the intended end users, to ensure that they are using the latest and most stable version of the product.

  To run the main (prod) locally, you need to execute the command "prod": "react-env --prefix UI_ENV --path './.env.prod' -- vue-cli-service serve"

  Link prod is https://onliner2.kraftds.com/#/

## Branches
App has three branches(according to the environment): 
 - development
 - stage
 - main (for prod)

To perform the release, you need to merge the stage into the main branch.
You can work both with dev and with stage in terms of development. You also need a branch from dev/stage

## Design
[This design](https://www.figma.com/design/i4wPyHzEsFeUPOhda2tQs7/Kraft---O2-(File---Share)?node-id=103-5313&t=j2pltbbztMGaZM3r-0) is the basis for implementing pages and components

## Additional documentation

[Backend documentation](https://gitlab.varteq.com/lirugo/kraft_2_backend)

