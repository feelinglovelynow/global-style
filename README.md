# 🕉 @feelinglovelynow/global-style


## 💎 Install
```bash
pnpm add @feelinglovelynow/global-style
```


## 💚 Use
```ts
import '@feelinglovelynow/global-style'
```

## 💛 Reasoning
* Common styling to ease web development
* Includes `html` styles to ease `rem` development - [additional information](https://stackoverflow.com/questions/59920538)
* Includes `fade in` and `fade in from above` animations
* Includes a class to show a loading circle
* Includes a couple of base classes like `fln__pr-text` which is helpful for adjacent `inline` elements when there is a desire for space between them like:
```html
<span class="fln__pr-text">Hello</span><a>World</a>
```


## 🧡 Loading circle implementation
```html
<div class="fln__circle-load"></div>
<div class="fln__circle-load blue"></div>

<style>
  .fln__circle-load { // gold load with transparent background
    border-color: #eac603 rgba(0, 0, 0, 0) rgba(0, 0, 0, 0);
  }

  .fln__circle-load.blue { // thicker + wider blue load with grey background
    border-width: 0.36rem;
    width: 4rem;
    border-color: #2e96ff #ccc #ccc;
  }
</style>
```


## ❤️ The Styles
```css
body,
html {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
}

html {
  font-size: 62.5%; /* https://stackoverflow.com/questions/59920538 */
}

body {
  font-size: 1.8rem;
  line-height: 1.369;
}

body * {
  box-sizing: border-box;
}

.fln__circle-load {
  width: 30px;
  aspect-ratio: 1/1;
  border-width: 0.27rem;
  border-style: solid;
  border-radius: 100%;
  animation: fln__circle-load__spin 0.8s infinite linear;
}

.fln__pr-text {
  padding-right: 0.45rem;
}

.fln__clear {
  clear: both;
}

.fln__relative {
  position: relative;
}

.fln__strong {
  font-weight: 600;
}

@keyframes fln__circle-load__spin {
  from {
    transform: rotate(0deg);
  }

  to {
    transform: rotate(359deg);
  }
}

@keyframes fln__fade-in {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes fln__fade-in-from-above {
  0% {
    opacity: 0;
    transform: translateY(-9rem);
  }

  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fln__fade-out-and-slide-up {
  0% {
    opacity: 1;
    transform: translateY(0);
  }

  100% {
    opacity: 0;
    transform: translateY(-9rem);
  }
}

@keyframes fln__subtle-fade-in-from-above {
  0% {
    opacity: 0;
    transform: translateY(-0.9rem);
  }

  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fln__subtle-fade-out-and-slide-up {
  0% {
    opacity: 1;
    transform: translateY(0);
  }

  100% {
    opacity: 0;
    transform: translateY(-0.9rem);
  }
}
```


## 🎁 All Our Packages
1. @feelinglovelynow/dgraph: [NPM](https://www.npmjs.com/package/@feelinglovelynow/dgraph) ⋅ [Github](https://github.com/feelinglovelynow/dgraph)
1. @feelinglovelynow/env-write: [NPM](https://www.npmjs.com/package/@feelinglovelynow/env-write) ⋅ [Github](https://github.com/feelinglovelynow/env-write)
1. @feelinglovelynow/get-form-entries: [NPM](https://www.npmjs.com/package/@feelinglovelynow/get-form-entries) ⋅ [Github](https://github.com/feelinglovelynow/get-form-entries)
1. @feelinglovelynow/get-relative-time: [NPM](https://www.npmjs.com/package/@feelinglovelynow/get-relative-time) ⋅ [Github](https://github.com/feelinglovelynow/get-relative-time)
1. @feelinglovelynow/global-style: [NPM](https://www.npmjs.com/package/@feelinglovelynow/global-style) ⋅ [Github](https://github.com/feelinglovelynow/global-style)
1. @feelinglovelynow/jwt: [NPM](https://www.npmjs.com/package/@feelinglovelynow/jwt) ⋅ [Github](https://github.com/feelinglovelynow/jwt)
1. @feelinglovelynow/loop-backwards: [NPM](https://www.npmjs.com/package/@feelinglovelynow/loop-backward) ⋅ [Github](https://github.com/feelinglovelynow/loop-backwards)
1. @feelinglovelynow/slug: [NPM](https://www.npmjs.com/package/@feelinglovelynow/slug) ⋅ [Github](https://github.com/feelinglovelynow/slug)
1. @feelinglovelynow/svelte-catch: [NPM](https://www.npmjs.com/package/@feelinglovelynow/svelte-catch) ⋅ [Github](https://github.com/feelinglovelynow/svelte-catch)
1. @feelinglovelynow/svelte-kv: [NPM](https://www.npmjs.com/package/@feelinglovelynow/svelte-kv) ⋅ [Github](https://github.com/feelinglovelynow/svelte-kv)
1. @feelinglovelynow/svelte-loading-anchor: [NPM](https://www.npmjs.com/package/@feelinglovelynow/svelte-loading-anchor) ⋅ [Github](https://github.com/feelinglovelynow/svelte-loading-anchor)
1. @feelinglovelynow/svelte-modal: [NPM](https://www.npmjs.com/package/@feelinglovelynow/svelte-modal) ⋅ [Github](https://github.com/feelinglovelynow/svelte-modal)
1. @feelinglovelynow/svelte-turnstile: [NPM](https://www.npmjs.com/package/@feelinglovelynow/svelte-turnstile) ⋅ [Github](https://github.com/feelinglovelynow/svelte-turnstile)
1. @feelinglovelynow/toast: [NPM](https://www.npmjs.com/package/@feelinglovelynow/toast) ⋅ [Github](https://github.com/feelinglovelynow/toast)
