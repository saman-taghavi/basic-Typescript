---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: true
# some information about the slides, markdown enabled
info: |
  ## Basic Typescipt
# persist drawings in exports and build
drawings:
  persist: false
monaco: true
---

# Basic Typescript

<div class="text-white rounded-md  font-black">
  <span @click="$slidev.nav.next" class="bg-blue-500   rounded cursor-pointer p-3" hover="bg-black bg-opacity-10 text-blue-500">
  hands on experince on basic typescript features
  </span>
</div>

<div class="absolute ">
<img src="https://avatars.githubusercontent.com/u/66922536" class="max-w-36  rounded-full mx-auto ">
<p>
Saman Taghavi
</p>
</div>

<!--
Ask audience about their prior knowledge
-->

---

<h1 class="font-bold text-blue-500 text-xl">
 What is Typescript?
</h1>

TypeScript is JavaScript with syntax for types.

- 🐞 **Errors** - some of them can be noticed before deployment
- 🎨 **Tools** - most Editors support it and have tools for it
- 🧑‍💻 **Developer Experience** - if You know it well enough otherwise use any
  ```ts {monaco}
  let s: any = "I don't care enough";
  ```
- 🤹 **Inference** - Typescript understands JS, it can infer when possible
- 🎥 **Progressive** - we can add it, incrementally and opt-in

```ts {1|2,3|all}
// @ts-check
function oh(array) {
  if (orray.length > 0) {
    return array;
  }
}
```

<br>
<br>
<span class="bg-white bg-opacity-20 right-5 p-5 absolute rounded-md " hover="bg-opacity-70 text-black">
Read more about <a class="text-blue-500"  href='https://www.typescriptlang.org/docs/handbook/intro.html' target=”_blank”>
Typescript
</a>
</span>

<style>
h1 {
  background-color: blue;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Code

Use code snippets and get the highlighting directly![^1]

```ts {all|2|1-6|9|all}
interface User {
  id: number;
  firstName: string;
  lastName: string;
  role: string;
}

function updateUser(id: number, update: User) {
  const user = getUser(id);
  const newUser = { ...user, ...update };
  saveUser(id, newUser);
}
```

[^1]: [Learn More](https://sli.dev/guide/syntax.html#line-highlighting)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---
layout: cover
class: text-center
image: https://source.unsplash.com/collection/94734566/1920x1080
---

<div>
Thank you
</div>
