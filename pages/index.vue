<script setup lang="ts">
import { appName } from '~/constants'
</script>

<template>
  <div class="page h-full flex flex-col items-center justify-center">
    <article class="p-4">
      <header class="mb-10">
        <h1 class="text-2xl mb-5 text-stone-500 font-semibold tracking-wide">
          {{ appName }}
        </h1>
        <h2 class="text-balance text-stone-600">
          Front-end engineer - mostly working with
          <IndexDescriptionLink to="https://www.typescriptlang.org/">
            TypeScript
          </IndexDescriptionLink>,
          <IndexDescriptionLink to="https://vuejs.org/">
            Vue.js
          </IndexDescriptionLink>,
          <IndexDescriptionLink to="https://nuxt.com/">
            Nuxt
          </IndexDescriptionLink>, and
          <IndexDescriptionLink to="https://tailwindcss.com/">
            Tailwind CSS
          </IndexDescriptionLink>
        </h2>
      </header>
      <main>
        <div class="links flex flex-col divide-y lg:flex-row lg:divide-y-0 lg:divide-x border rounded-md">
          <IndexLink to="https://github.com/dipodidae" target="_blank" icon="mingcute:github-fill">
            <span class="text-stone-400 group-hover:text-pink-400">github.com/</span>
            <span class="font-semibold">dipodidae</span>
          </IndexLink>
          <IndexLink to="mailto:tomvanveen@mail.com" icon="mingcute:send-line">
            <div class="flex gap-1 items-center">
              <span class="font-semibold">tomvanveen</span>
              <icon name="fa-solid:at" class="text-stone-400 group-hover:text-pink-400" />
              <span>mail.com</span>
            </div>
          </IndexLink>
          <IndexLink to="/resume.pdf" icon="mingcute:download-line">
            <span class="text-stone-400 group-hover:text-pink-400">view my</span> <span class="font-semibold">resume</span>
          </IndexLink>
        </div>
      </main>
    </article>
  </div>
</template>
