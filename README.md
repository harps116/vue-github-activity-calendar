# vue-github

> vue your github activity and calendar

[![Build](https://img.shields.io/travis/harps116/vue-github.svg?style=flat)](https://img.shields.io/travis/harps116/vue-github.svg?style=flat)
[![License](https://img.shields.io/npm/l/vue-github.svg?style=flat)](https://github.com/harps116/vue-github/blob/master/LICENSE.md)

[![NPM](https://nodei.co/npm/vue-github.png)](https://nodei.co/npm/vue-github/)

[Demo](https://harps116.github.io/vue-github/)

![](https://github.com/harps116/vue-github/raw/master/static/vue-github-screenshot.png)

## Installation

#### NPM

`npm i vue-github`

#### Yarn

`yarn add vue-github`

## Dependencies

Insert an octicons.css file in your html file to load the icons.

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/octicons/3.5.0/octicons.min.css"
/>
```

## Usage

Register the component globally in your main javascript file.

```javascript
import Vue from "vue";
import VueGithub from "vue-github";

Vue.use(VueGithub);
```

Check out the `main.js` in the [demo repo](https://github.com/harps116/vue-github/blob/master/demo/src/main.js).

import the style into your main `vue` file (most likely `App.vue`) if you want the default css.

```html
<style>
  @import url("https://unpkg.com/vue-github@0.10.7/dist/vueGithub.css");
</style>
```

In your template you can now use html like this to render the activity feed:

```html
<vue-github username="harps116" />
```

Props:

| name         | type    | default                                                                 | description                       |
| ------------ | ------- | ----------------------------------------------------------------------- | --------------------------------- |
| username     | String  | required                                                                | Github username                   |
| text         | String  | Summary of pull requests, issues opened, and commits made by {username} | Summary text                      |
| showCalendar | Boolean | true                                                                    | Whether to show the calendar      |
| showFeed     | Boolean | true                                                                    | Whether to show the activity feed |

## Issues

File issues [here](https://github.com/harps116/vue-github/issues)

## License

This project is licensed under MIT License - see the [LICENSE](./LICENSE.md) file for details

## Inspired by these great open source projects:

[https://github.com/IonicaBizau/github-calendar](https://github.com/IonicaBizau/github-calendar)

[https://github.com/lexmartinez/vue-github-activity](https://github.com/lexmartinez/vue-github-activity)
