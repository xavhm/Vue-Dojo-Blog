<template>
  <div class="post-list" v-for="post in posts" :key="post.id">
    <SinglePost :post="post" />
  </div>
</template>

<script>
import SinglePost from './SinglePost'

export default {
  props: ['posts'],
  components: {
    SinglePost
  }
}
</script>

<style>

</style>