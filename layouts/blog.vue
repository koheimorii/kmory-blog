<template>
  <div>
    <div class="container font-sans text-black">
      <main-navigation></main-navigation>
      <Nuxt class="markdown-body"/>
    </div>
  </div>
</template>

<script>
import { MainNavigation } from "../components/MainNavigation";

export default {
  comopnents: {
    MainNavigation,
  }
}
</script>

<style>
  @import url("https://cdnjs.cloudflare.com/ajax/libs/github-markdown-css/4.0.0/github-markdown.css");
  
  .markdown-body {
		box-sizing: border-box;
		min-width: 200px;
		max-width: 980px;
		margin: 0 auto;
		padding: 45px;
	}

	@media (max-width: 767px) {
		.markdown-body {
			padding: 15px;
		}
	}
</style>
