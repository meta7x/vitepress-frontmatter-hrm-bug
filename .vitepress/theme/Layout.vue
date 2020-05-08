<template>
  <div class="theme-container">
    <nav>
      <h1>{{ $site.title }}</h1>
      <p>{{ $site.description }}</p>
      <p>{{ $page.title }}</p>
      <p>{{ $page.frontmatter }}</p>
    </nav>
    <Content/>
  </div>
  <Debug/>
</template>

<script>
export default {
  created() {
    console.log(this.$page.frontmatter)
  }
}
</script>

<style>
h1 {
  color: grey;
}
</style>