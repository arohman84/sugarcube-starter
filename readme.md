# SugarCube Starter

The easiest starter kit for building SugarCube stories with Twine / Tweego.

## Features

- Automatic Tweego & SugarCube Install ✅
- Fully Configurable ✅
- Automatic Builds ✅
- Local server with Live Reload ✅
- Directory for custom fonts ✅
- Directory for third-party scripts ✅
- Up to date packages and frameworks ✅

## Tech Stack

Built in to this template are a number of frameworks to get you going.

- [Webpack v5](https://webpack.js.org/)
- [Babel](https://babeljs.io/) with [@babel/preset-env](https://babeljs.io/docs/en/babel-preset-env)
- [Sass](https://sass-lang.com/) with [Modern CSS Support](https://github.com/csstools/postcss-preset-env#readme) and [Font Magician Support](https://github.com/csstools/postcss-font-magician)

## Requirements

- Node.js 14+

## 🚀 Getting Started

1. Clone this repository: `npx degit nijikokun/sugarcube-starter <project-name>`
2. Run using `npm start`

## 👩‍💻 Commands

- `npm start` - Alias for `npm run dev`
- `npm run dev` - Starts development server and watches `src` directory.
- `npm run build` - Compiles and bundles the story in the `dist` directory.

## 📁 Directory Structure

- [`.build`](.build) — Webpack configuration and Build scripts
- [`src`](./src) — Story and Story Assets directory
- [`src/assets`](./src/assets) — Story Assets (Scripts, Styles, Media, Fonts)
- [`src/assets/app`](./src/assets/app) — Story JavaScripts and Stylesheets
- [`src/assets/app/styles`](./src/assets/app/styles) — Story Stylesheets (SASS)
- [`src/assets/fonts`](./src/assets/fonts) — Static Fonts to be hosted / distributed
- [`src/assets/media`](./src/assets/media) — Images and Videos
- [`src/assets/vendor`](./src/assets/vendor) — Third-Party Scripts and Modules
- [`src/story`](./src/story) — SugarCube / Twine `.twee` files
- [`config.json`](./config.json) — Webpack, Tweego, Babel and Build Configuration.

### Auto-Generated Directories

- `.tweego` — [Tweego](https://www.motoslave.net/tweego/) installation and story formats are installed here
- `.prebuilt` — Staging directory, files are processed and moved to `dist`
- `dist` — Compiled output directory

## 🙋‍♂️ How To

### How do I install macros?

Extract / place them into `src/assets/vendor`

### How do I link to media files?

Images and videos stored under `src/assets/media` get moved to the root directory under `media` which means that `favicon.png` ends up going from:

- `src/assets/media/favicon.png` → `media/favicon.png`

So to link to `favicon.png` you'd do ([`example`](./src/head-content.html)):

```html
<link rel="icon" type="image/png" href="media/favicon.png" />
```

### How do I add Google Analytics?

Paste the following snippet into [`src/head-content.html`](./src/head-content.html):

```html
<script
  async
  src="https://www.googletagmanager.com/gtag/js?id=YOUR_TAG_HERE"
></script>
```

and replace `YOUR_TAG_HERE` with your Google Analytics ID (`UA-########`).

## 🛣 Roadmap

- [x] Automatically install tweego for users so they don't have to.
- [ ] Add typescript support out of the box.
- [ ] Add configuration, commands and build process for production.
- [ ] Add support for compiling to Electron application.

## 🤝 Helpful Resources

- [Chapel's Custom Macro Collection](https://github.com/ChapelR/custom-macros-for-sugarcube-2)
- [Hogart's SugarCube Macros and Goodies](https://github.com/hogart/sugar-cube-utils)
- [SjoerdHekking's Custom Macros](https://github.com/SjoerdHekking/custom-macros-sugarcube2)
- [GwenTastic's Custom Macros](https://github.com/GwenTastic/Custom-Macros-for-Sugarcube)
- [Cycy Custom Macros](https://github.com/cyrusfirheir/cycy-wrote-custom-macros)
- [HiEv SugarCube Sample Code](https://qjzhvmqlzvoo5lqnrvuhmg-on.drv.tw/UInv/Sample_Code.html#Main%20Menu)
- [Akjosch SugarCube Resources](https://github.com/Akjosch/sugarcube-modules)
- [Mike Westhad SugarCube Resources](https://github.com/mikewesthad/twine-resources)
- [HiEv Universal Inventory](https://github.com/HiEv/UInv)

## Acknowledgements

We are grateful to these individuals for their ideas and contributions.

- [@ryceg](https://github.com/ryceg)

## License

Licensed under the MIT License.
