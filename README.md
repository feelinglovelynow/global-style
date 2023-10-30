# 🕉 @feelinglovelynow/global-style


## 💎 Install
```bash
pnpm add @feelinglovelynow/global-style
```


## 💚 Use
```ts
import '@feelinglovelynow/global-style'
```


## 💛 The Styles
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

.pr-text {
  padding-right: 0.45rem;
}

.clear {
  clear: both;
}

.relative {
  position: relative;
}

.strong {
  font-weight: 600;
}
```


## 🎁 All our NPM Packages
* [@feelinglovelynow/env-write](https://github.com/feelinglovelynow/env-write)
* [@feelinglovelynow/get-form-entries](https://github.com/feelinglovelynow/get-form-entries)
* [@feelinglovelynow/get-relative-time](https://github.com/feelinglovelynow/get-relative-time)
* [@feelinglovelynow/global-style](https://github.com/feelinglovelynow/global-style)
* [@feelinglovelynow/jwt](https://github.com/feelinglovelynow/jwt)
* [@feelinglovelynow/loop-backwards](https://github.com/feelinglovelynow/loop-backwards)
* [@feelinglovelynow/slug](https://github.com/feelinglovelynow/slug)
* [@feelinglovelynow/svelte-loading-anchor](https://github.com/feelinglovelynow/svelte-loading-anchor)
* [@feelinglovelynow/svelte-modal](https://github.com/feelinglovelynow/svelte-modal)
* [@feelinglovelynow/svelte-turnstile](https://github.com/feelinglovelynow/svelte-turnstile)
* [@feelinglovelynow/toast](https://github.com/feelinglovelynow/toast)
