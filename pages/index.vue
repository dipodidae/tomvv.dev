<script setup lang="ts">
import { appDescription, appName } from '~/constants'
</script>

<template>
  <article>
    <header>
      <h1>{{ appName }}</h1>
      <h2>{{ appDescription }}</h2>
    </header>
    <main>
      <div class="links">
        <NuxtLink to="https://github.com/dipodidae" target="_blank">
          <Icon name="mingcute:github-fill" /> github
        </NuxtLink>
        <span> | </span>
        <NuxtLink to="mailto:tomvanveen@mail.com">
          <Icon name="mingcute:send-line" /> tomvanveen@mail.com
        </NuxtLink>
        <span> | </span>
        <NuxtLink to="resume.pdf">
          <Icon name="mingcute:download-line" /> download my resume
        </NuxtLink>
      </div>
    </main>
  </article>
</template>
