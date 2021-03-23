<h1 align="center">Welcome to ohmyfood 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0.0-blue.svg?cacheSeconds=2592000" />
  <a href="https://github.com/ipopop/BaroniEmmanuel_3_03122020#readme" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
  </a>
  <a href="https://github.com/ipopop/BaroniEmmanuel_3_03122020/graphs/commit-activity" target="_blank">
    <img alt="Maintenance" src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" />
  </a>
</p>

> ohmyfood! Paris - "commander son menu au restaurant dès la reservation" - my version of a student project in OpenClassrooms (integration exercice with animations)

### 🏠 [Homepage](https://ipopop.github.io/BaroniEmmanuel_3_03122020/index.html)

![responsive](https://raw.githubusercontent.com/ipopop/BaroniEmmanuel_3_03122020/main/assets/img/pre-approved.jpg)
## Install

```sh
npm install
```
## Usage

### when dev on css, to run sass (watch only) :
```
npm run sass
```

### after sass & before save with git, prefix only (no watch) :
```
npm run prefix
```

### auto watch for sass & prefixer (watch) :
```
npm run watch:css
```

### scss tree (main sass file = 'scss/style.scss') :
```
scss
├── base
│   └── basics.scss
├── layouts
│   ├── _footer.scss
│   ├── _header.scss
│   └── _menus.scss
├── pages
│   ├── home-banner.scss
│   ├── home-nav-and-cards.scss
│   └── map-search-form.scss
├── partials
│   ├── _big-btn.scss
│   ├── _cards-anim.scss
│   ├── _icon-heart.scss
│   ├── _medias-queries.scss
│   ├── _menu-card.scss
│   ├── _sides.scss
│   ├── _spinner.scss
│   └── _spinner-heart.scss
├── style.scss
└── utils
    ├── mixins
    │   └── gradient-animations.scss
    └── variables
        └── colors.scss
```

### 'scripts' details from 'package.json' :
```
  "scripts": {
    "sass": "sass ./scss/style.scss:./css/style.css --watch --style compressed",
    "prefix": "postcss ./css/style.css --use autoprefixer -d ./css/prefixed/",

    "css:scss": "sass ./scss/style.scss:./css/style.css --style compressed",
    "css:autoprefixer": "postcss ./css/style.css -u autoprefixer -d ./css/prefixed/",
    "build:css": "npm run css:scss && npm run css:autoprefixer",
    "watch:css": "onchange \"scss\" -- npm run build:css"
  },
```
  and (for autoprefixer) :
```
  "browserslist": "last 4 versions",
```

### css tree :
```
css
├── prefixed
│   └── style.css
├── style.css
└── style.css.map
```

### html link to css :
```
<link rel="preload" href="css/prefixed/style.css" as="style">
<link rel="stylesheet" href="css/prefixed/style.css">
```

## Author

👤 **eb-dev**

* Website: maboite.space
* Github: [@ipopop](https://github.com/ipopop)

## Show your support

Give a ⭐️ if this project helped you!

## 📝 License

Copyright © 2021 [eb-dev](https://github.com/ipopop).<br />
This project is [MIT](https://en.wikipedia.org/wiki/MIT_License) licensed.

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_