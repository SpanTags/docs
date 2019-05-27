## Sphinx

Sphinx is a vuejs responsive dashboard built using vue-cli and vuetify.

-   [Live Demo](https://spantags.net/sphinx)

-   [Download Now](https://themeforest.net/user/spantags/portfolio)

## Contents

- [Sphinx](#sphinx)
- [Contents](#contents)
- [Prerequisites](#prerequisites)
- [Project setup](#project-setup)
    - [Compiles and hot-reloads for development](#compiles-and-hot-reloads-for-development)
    - [Compiles and minifies for production](#compiles-and-minifies-for-production)
- [Features](#features)
- [Pages](#pages)
- [UIKit](#uikit)
- [Layouts](#layouts)
    - [How to use layouts ?](#how-to-use-layouts)
- [Components](#components)
- [Views](#views)
- [Store](#store)
    - [Notes:](#notes)
- [Resources](#resources)
- [Final Thoughts](#final-thoughts)

## Prerequisites

**Sphinx** is built using modern workflow technologies and tools.

before using and developing **Sphinx** you should have the following tools installed on your system:

-   [nodejs](https://nodejs.org/). (required)
-   npm or [yarn](https://yarnpkg.com). (required)
-   git (optional)

## Project setup

After downloading the files from [here](https://spantags.net/sphinx) run the following commands:

`npm install` or `yarn install`

#### Compiles and hot-reloads for development

`npm run serve` or `yarn serve`

#### Compiles and minifies for production

`npm run build` or `yarn build`

## Features

-   material design concept
-   clean and elegant design.
-   Responsive layout.
-   dynamic switching among multiple layouts.
-   vuex and vue-router integration.
-   vast UIKIT (buttons, icons, cards, etc.)
-   material design icon set.
-   chartjs charts.
-   vuetify built-in charts.
-   mailbox, user profile and many prebuilt pages.

## Pages

-   dashboard
-   login/signup pages
-   user profile
-   notifications page
-   mailbox
-   calendar/events page
-   prices/plans page
-   many demo pages


## UIKit

**Sphinx** has an extensive collection of UI components containing:
- Material Cards.
- AutoCompletes, ComboBoxes, Selects, and author form controls.
- Buttons, Button Groups, Fabs
- Date Pickers
- Time Pickers
- Steppers
- Carousels
- Dialogs
- Chips
- Avatars
- Badges
- Sliders


## Layouts

**Sphinx** uses different page layouts for different purposes:

-   **default**: a layout with toolbar and standard left sidebar. (e.g. [dashboard](https://spantags.net/sphinx/dashboard))
-   **fullwidth**: a layout without the standard sidebar. (e.g. [mailbox](https://spantags.net/sphinx/mail))
-   **simple**: no toolbar, no sidebar. (e.g. [login](https://spantags.net/sphinx/auth/login))

#### How to use layouts ?

simply when you add a new route to the `router.js` file add a meta key like this:

```javascript
routes: [
    // ....
    {
        path: '/path/to/page',
        name: 'my example page',
        component: () => import('@/views/MyPage'),
        meta: { layout: 'simple' } // or default or fullwidth
    }
];
```

**Note** the `default` layout is used by default

## Components

The components folder contains reusable components.
Some of those components are loaded automatically and available application-wide with no need to import them, and some should be imported in order to use them as explained in the table below.

| Folder               | description                                                                                                                                                                                                                                                                                                            | Note                                                                                                                                                             |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `components/app`     | This folder contains the core components of the application like toolbar, drawer, panel, footer and thier partials.                                                                                                                                                                                                    | Those components are imported within the layout files.                                                                                                           |
| `components/chartjs` | This folder containes components that implements chartjs library charts like Pie, Line charts.                                                                                                                                                                                                                         | You have to import them withen your own components whenever you want to use them. you can find usage examples in [demo](https://spantags.net/sphinx/demo/charts) |
| `components/global`  | components in this folder and its sub folders are loaded automatically. you don't have to import them. example: if say you have a component called MyComponent inside a folder called `components/global/example`. then you can use the component any where like this: `<example-my-component></example-my-component>` | Note that: `components/global/example/MyComponent` became `example-my-component`.                                                                                |
| `components/demo`    | This folder contains components for demo purpose only.                                                                                                                                                                                                                                                                 | you can remove this folder before you go production. but before that you should remove references to them within other components and views.                     |

## Views

The `src/views/` folder containes the actual content visible to users.

those views are constructed from the reusable components from the `src/components` and from the core **vuetify** library.

## Store

**Sphinx** utilizes vuex as centeral store for app data.

#### Notes:

-   the modules under `store/modules` are added to the store automatically.
-   the `store/modules/demo` module is used in the demo. you can remove it before going production. but before that you should remove any references to it.
-   the `store/demo-data` is used in the `store/modules/demo` module. you can remove it after removing the `store/modules/demo` module.

## Resources

**Shinx** is built using a set of awesome tools and libraries.

So you may refer to thier own documentation for more insight.

-   [Vue](https://vuejs.org/)
-   [Vuetify](https://vuetifyjs.com/)
-   [Vuex](https://vuex.vuejs.org/)
-   [Vue-router](https://router.vuejs.org/)
-   [Vue-chartjs](https://vue-chartjs.org/)

## Final Thoughts

Don't hesitate to ask us for help.

you can contact us through the themeforest contact form [here](https://themeforest.net/user/spantags).

you can download the templete from [here](https://themeforest.net/user/spantags/portfolio).
