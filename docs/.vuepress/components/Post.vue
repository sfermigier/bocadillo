<template>
  <Page :sidebarItems="[]">
    <template slot="top">
      <p class="wrapper">
        <router-link to="/blog/">← Back to posts</router-link>
      </p>

      <PostShare :page="$page"/>

      <PostJumbotron :post="$page.frontmatter"/>

      <div class="wrapper">
        <hr>
      </div>
    </template>
  </Page>
</template>

<script>
import Page from "@theme/Page";
import PostShare from "./PostShare";

export default { components: { Page, PostShare } };
</script>
